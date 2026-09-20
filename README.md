# Research Scout

**Research Scout** is a focused AI skill for gathering and preserving verifiable research evidence. It collects sources and faithfully records what they say; it does **not** interpret, rank, recommend, diagnose, or draw conclusions.

This package is designed for beginners. Upload the whole folder to Google Drive (or another persistent workspace), then connect it to an AI agent that can read and update its files.

## What it does

- Creates one durable memory file per research topic.
- Searches approved source types through modular provider wrappers.
- Saves source details, relevant excerpts, dates, URLs, and collection notes.
- Detects obvious duplicates and preserves a simple research log.
- Returns a factual evidence inventory rather than an opinion or report.

## What it deliberately does not do

- Analyse evidence or explain what it means.
- Recommend a product, decision, treatment, strategy, or action.
- Score sources, make a literature review, or produce an executive conclusion.
- Invent citations, quotations, URLs, or findings.

## Package map

```text
Research-Scout-Skill/
├── README.md              Start here
├── SKILL.md               Instructions for the AI agent
├── MANUAL.md              Beginner guide (40 lesson pages)
├── TEMPLATE.md            Blank memory-file template
├── manifest.json          Package metadata
├── providers.md           Provider wrapper catalogue
├── memory/
│   └── .gitkeep           Topic memory files live here
└── tools/
    ├── README.md          Wrapper contract and examples
    └── .gitkeep           Add provider wrappers here
```

## Quick start

1. Keep the entire folder together in Google Drive; do not move `memory/` away from the other files.
2. Give your AI agent access to the folder and ask it to read `SKILL.md` before doing work.
3. Make a request such as: “Use Research Scout to collect evidence about vertical farming energy use. Store it in topic `vertical-farming-energy`.”
4. The agent creates `memory/vertical-farming-energy.md` by copying `TEMPLATE.md`, gathers evidence, and appends records.
5. Open the memory file whenever you need the collected material. Ask a separate analysis skill or person to interpret it.

## Safe request examples

- “Collect peer-reviewed evidence on sleep duration in adolescents. Do not analyse it.”
- “Add official New Zealand government guidance on flood preparedness to `flood-preparedness-nz`.”
- “Show the source list currently saved for `urban-trees`.”

## Upload to Google Drive

Upload `Research-Scout-Skill.zip`, extract it in Drive, and keep the resulting folder intact. A shortcut or shared-drive folder is fine as long as the agent has permission to read and update files, particularly `memory/`.

For a full walkthrough, read [MANUAL.md](MANUAL.md).
