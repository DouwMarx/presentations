# Presentations

A collection of reveal.js presentations hosted via GitHub Pages. Each presentation lives on its own branch and is merged into `master` for deployment.

## Viewing Presentations

Presentations are available at:
```
https://douwmarx.github.io/presentations/index.html
```

## Creating a New Presentation

1. Create an orphan branch from master:
   ```bash
   git checkout master
   git checkout --orphan my-new-presentation
   git reset --hard
   ```

2. Create your `index.html` (use an existing presentation branch as a template).

3. Commit and merge back to master:
   ```bash
   git add .
   git commit -m 'Initial commit for my-new-presentation'
   git checkout master
   git merge my-new-presentation --allow-unrelated-histories
   git push --all origin
   ```

## Updating reveal.js

To pull the latest reveal.js changes:
```bash
git checkout master
git pull upstream master
git push origin master
```

## Current Presentations

| Branch | Topic |
|--------|-------|
| `data-science-leuven-reward-models-ais` | Reward Models & AI Safety (Leuven Data Science Meetup) |
