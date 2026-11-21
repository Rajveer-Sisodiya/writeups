# Writeups

Source for the writeups shown on https://ravansec.publicvm.com/writeups

## Folders

One folder per platform. Each folder becomes a folder in the left sidebar of the site.

```
offsec/         OffSec (Proving Grounds, PEN-200 labs)
tryhackme/      TryHackMe
hackthebox/     Hack The Box
hacksmarter/    Hack Smarter
```

Create more folders any time (for example `portswigger/` or `picoctf/`). Sub-folders work too, for example `hackthebox/windows/`.

## Adding a writeup

1. Copy `_templates/writeup-template.md` into the right folder and rename it, for example `tryhackme/blue.md`.
2. Fill in the front matter (title, platform, difficulty, date, tags, summary) and write the sections.
3. Put screenshots in an `images/` folder next to the file and reference them as `![alt](images/name.png)`.
4. Commit and push. The site picks it up within about 5 minutes.

Files starting with `_` or `.` and README files are never published. Add `draft: true` to the front matter to hide a writeup while you work on it.

## Rules

Only publish writeups for labs, CTFs and systems you are allowed to test. Never include real client data, live credentials or flags from active competitions.
