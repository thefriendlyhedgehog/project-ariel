# Community sources

Raw material pulled in from outside GitHub — Discord exports, forum threads,
vendor posts — that the rest of project-ariel's documentation (in particular
`arieltune/crates/bc250-catalog/src/bc250_manual.md`) cites or draws on.

This folder holds the material itself, not conclusions drawn from it. When a
finding from something in here gets folded into the manual or another doc,
that doc cites back to the specific file here.

## Layout

```
discord/
  <short-topic>-<year>-<month>/   # one folder per export
    export.json                  # DiscordChatExporter output (or .html)
    attachments/                 # files posted alongside (BIOS images, etc.)
forums/
  <same pattern, for non-Discord sources>
```

## Adding a new source

Each export folder should note, either in a short `NOTES.md` inside it or in
the commit message that adds it:

- **Source**: which server/channel, or which forum/thread
- **Authorization**: who gave permission to export and share this (a
  moderator, the server owner, the original poster) — Discord content in
  particular should only go here if whoever runs the server has agreed
- **Date exported**
- **Why it's here**: what it's expected to be useful for

One folder per server (or per thread), not per person who did the exporting —
if two people independently export the same server, that's one source folder,
not two.
