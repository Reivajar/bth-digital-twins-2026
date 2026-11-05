# Start here

A working 3D map of central Helsingborg that you change by talking to an AI assistant. Nothing to install.

## 1. Open it (Monday, 5 minutes)

1. Unzip the folder somewhere you can find it, for example your Desktop. Do not open it from inside the zip.
2. Double-click `index.html`. It opens in your browser.
3. You should see 3D buildings, a slider on the right, and a number that changes when you move the slider.

If you see a blank page, try Chrome or Edge. If it is still blank, tell Javier in the Monday online check.

## 2. What is in the folder

| File | What it is | Do you edit it? |
| --- | --- | --- |
| `index.html` | The page: map, panel, and the function | Yes, through the AI assistant |
| `data/buildings.js` | About 5,200 buildings with height, use, ground elevation | No. Never paste it into the AI chat |
| `data/context.js` | Water and parks for the background | No |
| `lib/` | The map library | No |
| `docs/PROMPTS.md` | Prompts to start each project option | Read it |
| `docs/DATA.md` | What each data field means and how reliable it is | Read it before writing your brief |
| `docs/requirement-brief-template.docx` | Template for your main deliverable | Yes, this is where your grade comes from |

## 3. How to change it with AI

1. Open `index.html` in a text editor (Notepad, TextEdit in plain-text mode, or VS Code). Select all and copy.
2. In the AI chat, paste the instruction from `docs/PROMPTS.md`, then the whole `index.html`.
3. Ask for **the complete file back**, not a fragment.
4. Paste the answer over the contents of `index.html`, save, and reload the browser.

## 4. Three rules

- **Save a numbered copy each time it works.** `v1.html`, `v2.html`, and so on, in the same folder. When the AI breaks the page, open the last copy and start again from there. This is your undo button.
- **Never paste the data files into the chat.** They are too big. The AI only needs to know the field names, which are in `docs/DATA.md`.
- **Write down what went wrong.** Every time the AI gets something wrong, add one line to your build log: what you asked, what it did, what you changed.

## 5. When it breaks

1. Blank page: open the browser console (F12 on Windows, Cmd+Option+J on Mac), copy the red error message, paste it into the AI chat and ask it to fix the error.
2. Still broken after two tries: go back to your last numbered copy.
3. Still stuck: ask another group, then Javier.
