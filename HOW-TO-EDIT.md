# How to edit the website

You don't need to know how to code. All the things you'll want to
change are marked in the files with `EDIT:` comments.

There are three ways to edit, from easiest to most technical.

## Option 1 — Edit on GitHub (easiest, recommended for your professor)

Once the site is on GitHub (see DEPLOY.md):

1. Go to your GitHub repository in a web browser.
2. Click the file you want to change (for example, `index.html`).
3. Click the small pencil icon ("Edit this file") in the top right.
4. Use `Ctrl+F` / `Cmd+F` to find text you want to change (for example,
   search for `meiser@up.edu` to change the professor's email).
5. Scroll to the bottom, write a short note like "Updated email", and
   click **Commit changes**.
6. Within about a minute, the live website updates automatically.

No software to install. Works from any computer.

## Option 2 — Edit on your computer

1. Download the folder to your computer.
2. Open `index.html` in any text editor. Free options:
   - **VS Code** (recommended) — https://code.visualstudio.com
   - **TextEdit** (Mac) — use Format → Make Plain Text
   - **Notepad** (Windows)
3. Find the `EDIT:` comments and change the text between tags.
4. Save the file.
5. Double-click `index.html` to preview in your browser.
6. Upload the changed file back to GitHub.

## Option 3 — Common edits (cheat sheet)

### Change the professor's email
Search for `meiser@up.edu` in `index.html` and replace it (it appears
in the Contact section and in the footer).

### Add a new paper
In `index.html`, find the Research section. Copy one of the
`<a class="paper">...</a>` blocks and paste it below. Change the title,
author, abstract, and the filename in `href="papers/..."`.

Then make a new HTML file for the paper — the easiest way is to copy
one of the existing files in the `papers/` folder, rename it, and
change the text.

### Add a new leadership member
In `index.html`, find the Leadership section. Copy one of the
`<div class="person">...</div>` blocks and change the role, name,
and title.

### Change how fast the background photos switch
In `index.html`, near the bottom, find the line:

```
}, 6000);
```

Change `6000` to a different number. That's in milliseconds — 6000 is
6 seconds, 10000 is 10 seconds.

### Change the photos
Put new photos in the `images/` folder, named `campus-1.jpg` through
`campus-4.jpg`. See `images/README.txt` for details.

### Change the group name or the Kelly quote
In `index.html`, look near the top of the HERO section. They're
marked with `EDIT:` comments.
