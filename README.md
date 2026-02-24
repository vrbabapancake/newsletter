# Monthly Newsletter

A Jekyll-based static site for publishing monthly newsletter issues.

## Setup

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Adding a New Issue

Create a new file in `_newsletters/` following the naming convention:

```
_newsletters/YYYY-MM-DD-month-year.md
```

Use this front matter template:

```yaml
---
issue: 2
title: "March 2026"
date: 2026-03-01
description: "A short teaser shown on the index page."
---
```

Then write the issue body in Markdown below the front matter.

## Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/
│   ├── default.html     # Base layout
│   └── newsletter.html  # Per-issue layout
├── _newsletters/        # One .md file per issue
├── assets/css/
│   └── style.css        # Styles
└── index.html           # Issue listing page
```
