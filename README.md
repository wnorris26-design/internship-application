# Internship Command Center

A personal tool for Wyatt Norris's summer 2027 internship search.

**Live app:** https://claude.ai/artifact/HbdxR94pKF9zZUiCUE7vAU (private to its owner)

## What it does

- **Tracker**: every posting, sorted by deadline, with countdown chips, status (Watching → To apply → Applied → Interviewing → Offer), notes and links. Filter by area (Healthcare, Operations, Corporate, Consulting). Changes save to the artifact's database.
- **Fit check**: paste a job posting and Claude scores how it fits your resume, requirement by requirement. It flags gaps and eligibility issues (graduation dates, location) and won't count skills you don't have.
- **Cover letter**: drafts a tailored letter in your voice from one of three templates (Healthcare, Operations / supply chain, Customer / AI). It also works offline as a plain fill-in-the-blanks template.

## Files

- `app/index.html`: the app (published as a claude.ai artifact)
- `data/internships.json`: the starter list of 20 postings researched Nov 19, 2026. The live tracker is the source of truth after that. This file is the offline fallback.

## Updating

Ask Claude Code to "add postings to my internship tracker" or "update the status of X". It writes to the artifact's database directly, so the page doesn't need to be republished.
