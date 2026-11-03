# Contributing as a team

Welcome! This repository is a learning project. Keep contributions focused so classmates can review and understand each other's work.

## Before you start

- Make sure you have Git installed and can access the repository on GitHub.
- Never commit passwords, access tokens, private student information, or other secrets.
- Coordinate with your group before editing the same section or shared stylesheet.

## Recommended workflow

### 1. Sync your local copy

```bash
git switch main
git pull origin main
```

### 2. Create a branch for your task

Use a short, descriptive name. Prefixes such as `feature/`, `fix/`, and `docs/` make the purpose clear.

```bash
git switch -c feature/testimonials
```

Avoid working directly on `main`.

### 3. Make a focused change

- Keep each branch about one feature, fix, or documentation update.
- Use semantic HTML elements where appropriate.
- Keep CSS organized and reuse the existing custom properties in `:root`.
- Check the page at a narrow mobile width and a wider desktop width.
- Do not add a library or build system without agreeing with the team first.

### 4. Review and commit your work

```bash
git status
git diff
git add index.html css/style.css
# Stage only the files you changed; adjust the command as needed.
git commit -m "Add testimonial section"
```

Write commit messages that describe the change, such as `Fix card spacing on mobile` or `Add provider profile section`.

### 5. Push your branch and open a pull request

```bash
git push -u origin feature/testimonials
```

On GitHub, open a pull request from your branch into `main`. In the description, explain what you changed, how someone can review it, and any known follow-up work. Add before/after screenshots for visible design changes when possible.

Ask a classmate to review the pull request. Respond to feedback with additional commits on the same branch. Once approved, merge it using the class's chosen merge method.

### 6. Clean up after merge

```bash
git switch main
git pull origin main
git branch -d feature/testimonials
```

## Pull request checklist

- [ ] The change has one clear purpose and a descriptive title.
- [ ] The page still opens without errors and no unrelated files changed.
- [ ] I checked the layout on mobile and desktop.
- [ ] Links, headings, and images have meaningful text or alternatives.
- [ ] I added no credentials, personal data, or unlicensed assets.
- [ ] The pull request explains the change and includes screenshots when useful.
