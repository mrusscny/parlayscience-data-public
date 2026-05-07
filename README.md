# ParlayScience Data Public

Auto-generated daily JSON outputs from the ParlayScience MLB data pipeline. Used by the figma plugin for content auto-fill.

## Layout

```
outputs/
├── YYYY-MM-DD/        # one folder per pipeline run date (UTC)
│   └── *.json         # concept JSON files (e.g. nrfi_matchups.json)
└── latest/            # mirror of the most recent successful run
    └── *.json
```

The figma plugin fetches `outputs/<today>/nrfi_matchups.json` (today in UTC). Files appear here automatically after each pipeline run on the private upstream repo.
