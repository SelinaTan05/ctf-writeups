# Metamon3

| Competition | Category | Solved by |
| --- | --- | --- |
| UMCS CTF 2026 | DFIR | [@SelinaTan05](https://github.com/SelinaTan05) |

## The Solve

After identifying the suspicious browser activity in Metamon2, I checked the user's temporary directory for files related to the incident:

```text
Users\ahmad\AppData\Local\Temp\
```

I looked for unusual files around **19 April 2026** and found two batch files, `rizzler.bat` and `sentineltwo.bat`.

I opened `rizzler.bat` in FTK Imager's text view. Near the beginning, the script set its target to `%TEMP%\sentineltwo.bat` and copied itself there:

```bat
set "target=%TEMP%\sentineltwo.bat"
copy "%~f0" "%target%" /Y >nul
```

That connected the two filenames: `%~f0` refers to the running batch file, so the second file was a copy made by the script rather than an unrelated artifact.

![Batch script in the temporary directory](images/image1.png)

Further down, the script contained registry commands involving `HKCU\Software\Classes\ms-settings\CurVer`, followed by a call to `fodhelper.exe`. The flag was already visible as a string in one of those registry commands. I copied it from the text view without running the batch file.

## Flag

```text
UMCS{Ra-T4-TA-Ta_BU7_1_doN7_w4nT_tO}
```

[Previous: Metamon2](../Metamon2/README.md) · [Back to UMCS CTF](../../README.md)
