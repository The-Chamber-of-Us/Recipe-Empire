# Git Workflow Guide – Recipe Empire

This document outlines how we use Git and GitHub to collaborate efficiently on the Recipe Empire project.

---

## ✅ Branch Naming Convention

Always create a new branch from `main` when starting work.

Use prefixes based on the type of task:

| Prefix      | Purpose                      | Example                        |
|-------------|------------------------------|--------------------------------|
| `feature/`  | New features                 | `feature/recipe-form`          |
| `bugfix/`   | Bug fixes                    | `bugfix/fix-image-upload`      |
| `style/`    | Styling and layout changes   | `style/update-landing-page`    |
| `docs/`     | Documentation updates        | `docs/git-workflow-guide`      |

---

## 💬 Commit Messages

Write clear and meaningful messages. Keep it short but descriptive.

**Good examples:**
- `Add recipe form component`
- `Fix image upload error on mobile`
- `Update styles for recipe card`

**Avoid:**
- `changes`
- `update`
- `final fix`

---

## 🔀 Pull Requests

- Open a pull request to merge your branch into `main`
- Use the format: `Title of the feature – what it does`
- Link to the related issue (e.g., `Closes #3`)
- Request a review if you're unsure about something
- Don’t push directly to `main`

---

## 🔁 Keeping Your Branch Updated

Before starting a new branch:

```bash
git checkout main
git pull origin main
git checkout -b feature/your-feature
```


## If your branch gets outdated:

```bash
git checkout main
git pull origin main
git checkout your-branch
git merge main
```

⚠️ Conflict Handling
If you see merge conflicts, don’t panic.

Ask for help or ping someone with experience before resolving it.

Never commit conflict markers (like <<<< HEAD).

📦 Clean-Up
After merging your pull request:

```bash
git branch -d your-branch
git push origin --delete your-branch
```
Let’s keep the repo clean!

Happy coding! 💚
