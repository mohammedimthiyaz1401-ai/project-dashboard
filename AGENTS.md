# Project Dashboard - AGENTS.md

## What
Personal project dashboard with MEOW chat assistant. Shows all project statuses, YouTube channels, emails, URLs, book upload status, LinkedIn content ideas.

## Tech Stack
- Single-page HTML/JS (no framework)
- Orbitron + Rajdhani fonts
- Sunset sky theme with clouds
- GitHub Pages hosting

## Key Files
- index.html - Everything (sections, MEOW assistant, YouTube status checker, URL tracker)

## Sections (in order)
1. Header (name, title, location)
2. Stats Row (repos, channels, books, websites, emails)
3. YouTube & Rumble Status
4. Quick Links
5. Websites & Portfolio
6. Infrastructure
7. Future Tools to Adopt
8. LinkedIn Content (8 trending topics + weekly schedule)
9. Email Accounts (with copy buttons)
10. GitHub Repositories
11. Book Upload & Prompts
12. Project URLs

## How to Deploy
```
git push origin main
# Auto-deploys to GitHub Pages
```

## How to Add a Section
1. Add HTML div with class="section" data-section="name"
2. Add to scrollTo map in JS (line ~1064)
3. Add to websiteControl sections map (line ~945)
4. Add to hide/show commands in MEOW

## MEOW Commands
- tasks: add/list/complete/remove task
- notes: add/list/delete note
- reminders: remind me... in X min
- timer: start/stop timer
- calculator: calculate 2+2
- converter: convert 5 km to miles
- URLs: list/add/remove/open url
- weather/joke/quote/news
- scroll to [section]
- hide/show [section]
- themes: apply [theme]

## Dashboard Rules
- New repo: Add to Quick Links, GitHub Repos, PROJECT URLS
- New email: Add to Email Accounts section
- New YouTube channel: Add to YT_REPOS in checkYouTubeStatus()
- Project status change: Update badge
- Always commit + push after edits

## LinkedIn Content Section
- 8 trending topics with post ideas, hashtags
- Weekly schedule: Mon-Sun topic rotation
- Best times: 8-10 AM or 5-7 PM IST

## .gitignore
None needed (single HTML file, no secrets)
