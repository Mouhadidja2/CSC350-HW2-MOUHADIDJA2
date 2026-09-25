# Homework 2 — Part 2: Requirements Derived from Git Commands

Your task is to describe what a Git-like version-control system must provide from the user's perspective.

## Part 1 — Git command observations

Choose **four** Git commands or closely related command workflows that you practiced. For each selection, record what happened, what the user was trying to accomplish, and what problem or risk it addressed.

## Part 2 — User needs

Write at least **Three user needs** based on the observations. The more, the better.

Use this pattern:

> **UN-GIT-01:** A `[type of user]` needs a way to `[desired outcome]` because `[problem or reason]`.

Each need must identify a role, desired outcome, and reason; remain solution-independent; and avoid naming a Git command.

## Part 3 — User requirements

Write at least **Four user requirements** derived from the user needs. The more, the better.

Use this pattern:

> **UR-GIT-01:** A `[user role]` shall be able to `[user-visible capability]` `[necessary condition]`.

Each requirement must describe one user-visible capability and trace to a user need. Complete the answer sheet in `submissions/homework-2/GIT_REQUIREMENTS.md`.

## Submission instructions

**Instructor repository:**

<https://github.com/elmtang/minigit-course-project>

### Step A — Fork the repository

1. Open the instructor repository using the link above.
2. Select **Fork**.
3. Keep the repository name:

   ```text
   minigit-course-project
   ```

The fork belongs to your GitHub account. You will submit your work to your fork, not directly to the instructor repository.

### Step B — Clone your fork

Replace `STUDENT-USERNAME` with your GitHub username:

```bash
git clone https://github.com/STUDENT-USERNAME/minigit-course-project.git
cd minigit-course-project
```

Cloning your fork automatically names it `origin`.

### Step C — Add the instructor repository

Add the instructor repository as `upstream`:

```bash
git remote add upstream https://github.com/INSTRUCTOR-USERNAME/minigit-course-project.git
git remote -v
```

The output should identify:

```text
origin     your forked student repository
upstream   the instructor repository
```

You will push your work to `origin`. You will use `upstream` to obtain new homework instructions and instructor-provided files later in the course.

### Step D — Create the Homework 2 answer file

Copy:

```text
assignments/homework-2/GIT_REQUIREMENTS_TEMPLATE.md
```

to:

```text
submissions/homework-2/GIT_REQUIREMENTS.md
```

You may use this command:

```bash
cp assignments/homework-2/GIT_REQUIREMENTS_TEMPLATE.md submissions/homework-2/GIT_REQUIREMENTS.md
```

Complete all sections in the copied file. Do not place your answers in the template under `assignments/`.

### Step E — Commit and push the answer

Inspect your work before committing it:

```bash
git status
git diff
git add submissions/homework-2/GIT_REQUIREMENTS.md
git diff --staged
git commit -m "Complete Homework 2 Part 2"
git push origin main
```

### Step F — Mark the submitted version

After pushing the final version, create and push the submission tag:

```bash
git tag hw2-submission
git push origin hw2-submission
```

If you already created `hw2-submission`, do not move or replace it unless the instructor has authorized a resubmission.

## What to submit through the LMS

Submit all of the following to your Google classroom (NOT here):

- Your fork URL, for example: `https://github.com/STUDENT-USERNAME/minigit-course-project`
- List of files that you updated for this homework
- The full commit ID of your submitted version
- Confirmation that you pushed the `hw2-submission` tag

Obtain the full commit ID with:

```bash
git rev-parse HEAD
```

Before submitting, open your fork on GitHub and verify that:

- `submissions/homework-2/GIT_REQUIREMENTS.md` contains your final answers.
- The commit appears in the repository history.
- The `hw2-submission` tag appears in the repository.
- You did not edit `assignments/homework-2/GIT_REQUIREMENTS_TEMPLATE.md`.
