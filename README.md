# CTF Writeups

A collection of writeups, solve scripts, and lessons learned from past Capture the Flag competitions.

## Competition Index

| Year | Competition | Writeups |
| --- | --- | --- |
| 2026 | UMCS CTF | [View writeups](UMCS%20CTF/README.md) |

## Repository Structure

Organize writeups by competition and category, with a separate folder for each challenge:

```text
UMCS CTF/
├── README.md                  # Competition index
└── Web/
    └── Challenge Name/
        ├── README.md          # Walkthrough and explanation
        ├── images/
        │   ├── image1.png
        │   └── image2.png
        └── solve.py           # Solve script, if available
templates/
└── writeup.md
```

## Adding a Writeup

1. Create a challenge folder under `Competition Name/Category/Challenge Name/`.
2. Copy `templates/writeup.md` into the challenge folder as `README.md`.
3. Save screenshots in `images/` as `image1`, `image2`, and so on, preserving their file extensions. Restart numbering for each challenge. Include original challenge files in `attachments/` and solve scripts alongside the writeup, when available.
4. Add a link to the competition in the index above.

Credit the original solver in each writeup. Add a GitHub profile link only when the account is confirmed, and cite any external writeups used.

In VS Code, press `Ctrl+Shift+V` while editing a Markdown file to preview it.
