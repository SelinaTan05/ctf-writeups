# Ghost in the Repo 1 - GCTF 2026

Solved by [@SelinaTan05](https://github.com/SelinaTan05)

## The Solve

First I first used `git log --oneline` to inspect the normal commit history, but the commit containing the password was not listed.
![alt text](images/image1.png)

I then checked the Git reference log. Then I found where the db password added.
![alt text](images/image2.png)

Then, inspect the removed commit named `"fix: added db password"`.
![alt text](images/image3.png)

`gctf26{db_p4ss_qw3r1234!}`

[Original writeup](https://github.com/adrianchx/writeups/blob/ecf3fcff2316415cb6b089dd1879e544482a0ea9/2026-10-02_GCTF-2026/forensics/ghost-in-the-repo-1/README.md) · [Back to GCTF 2026](../../README.md)
