# Field Notes — AI as subject-matter expert

A swipeable short-form reader for the AI-SME research series.

## Read it online

**[Open the live GitHub Pages site](https://automationscompany.github.io/ai-sme-swipe/)**

The site is publicly hosted by GitHub Pages. You do not need to run anything locally to access it.

- Live site: https://automationscompany.github.io/ai-sme-swipe/
- Repository: https://github.com/automationscompany/ai-sme-swipe

## What it contains

- Swipeable cards distilled from the Waterware, Multiquip, and Pooldoktor case studies
- Multiple cards per source article
- Touch, keyboard-arrow, and button navigation
- Filters for each case study
- Direct links back to the source articles
- A cross-case thread tracking automation, human escalation, safety boundaries, and digital-company-twin evidence

## Publishing updates

The repository uses GitHub Actions to deploy the contents of `main` to GitHub Pages. After editing the site:

```bash
git add .
git commit -m "Update research cards"
git push
```

The workflow will redeploy the live site automatically. Check deployment status in the repository’s **Actions** tab.

## Optional local preview

Local hosting is only needed when developing or testing changes before publishing. It runs on the machine where you execute the command; it is not the public site and other people cannot access it unless that machine is separately exposed to the network.

```bash
cd /data/workspace/ai-sme-swipe
python3 -m http.server 8765
```

Then open http://localhost:8765 on that same machine. Stop the server with `Ctrl+C`.
