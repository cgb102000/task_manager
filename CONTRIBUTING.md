# Contributing to DevBoard

Welcome! DevBoard is an open-hours project built on top of the [Navas Task Manager API](https://dev.to/navas_herbert/building-a-rest-api-with-fastapi-from-scratch-full-crud-sqlite-middleware-cors-j92).
The goal is to evolve a basic FastAPI CRUD app into a full collaborative task board, one pull request at a time.

Every merged contribution is a real open source commit on your GitHub profile.

## Table of contents

- [Before you start](#before-you-start)
- [1. Fork and clone the repository](#1-fork-and-clone-the-repository)
- [2. Create a branch](#2-create-a-branch)
- [3. Make your changes](#3-make-your-changes)
- [4. Commit and push](#4-commit-and-push)
- [5. Open a pull request](#5-open-a-pull-request)
- [Pull request checklist](#pull-request-checklist)
- [Picking an issue](#picking-an-issue)
- [Questions?](#questions)

## Before you start

- Pick one issue and comment on it before you begin so others know it is being worked on.
- Keep your work focused on a single problem or feature.
- If you want to work on more than one issue, open separate branches and pull requests for each one.

## 1. Fork and clone the repository

Click the Fork button at the top-right of the repository page, then clone your fork locally:

```bash
git clone git@github.com:YOUR_USERNAME/task_manager.git
cd task_manager
```

## 2. Create a branch

Use a branch name that matches the issue you are solving:

```bash
git checkout -b feature/your-issue-name
# examples:
# feature/add-priority-field
# fix/pagination-off-by-one
# docs/contributing-guide
```

Keep one pull request per issue. If your work covers more than one issue, split it into separate branches and pull requests.

## 3. Make your changes

- Keep the changes focused on the issue you selected.
- Follow the existing project style, including snake_case, type hints, and Pydantic schemas.
- Test your changes locally before submitting.
- Update the README if a new endpoint or behavior changes how the project is used.

## 4. Commit and push

Use a clear commit message that explains what changed:

```bash
git add .
git commit -m "feat: add priority field to Task model (#1)"
git push origin feature/your-issue-name
```

Common prefixes:

- `feat:` - new feature
- `fix:` - bug fix
- `docs:` - documentation only
- `test:` - adding or updating tests
- `refactor:` - code change without changing behavior

## 5. Open a pull request

Open a pull request against the main branch of Navashub/task_manager.

Your PR description should clearly explain:

- what changed
- which issue it addresses
- any tests or checks you ran

## Pull request checklist

Before submitting, make sure:

- [ ] The app still runs locally (`uvicorn main:app --reload`)
- [ ] The relevant endpoints appear and work in `/docs`
- [ ] Your changes do not introduce unused imports or dead code
- [ ] The README was updated if behavior or endpoints changed
- [ ] The branch name matches the issue being solved
- [ ] The pull request is focused on one issue

## Picking an issue

Issues are labelled by difficulty:

| Label | Who it's for |
|---|---|
| `good-first-issue` | Just getting started with FastAPI |
| `intermediate` | Comfortable with models, schemas, and routers |
| `advanced` | Ready for auth, testing, or DevOps |
| `frontend` | HTML/CSS/JS or React work |
| `devops` | Docker, PostgreSQL, deployment |

Comment on an issue before starting so others know it is being worked on.

## Questions?

Reach out on WhatsApp or open a GitHub Discussion. Don't be afraid to ask - that's what open hours is for.
