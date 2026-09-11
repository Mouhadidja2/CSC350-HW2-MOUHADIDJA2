# Homework 2 — Independent Festival Visitor Guide

## Purpose

Complete this homework independently in the separate repository provided. Demonstrate that you can select and use the appropriate Git and GitHub commands learned in Activities 01 and 02.

This homework must not modify the pair repository used for Activities 03–08.

## Estimated time

60–75 minutes

## Available resources

You may consult the lecture slides, Lab 1 and Lab 2 materials, and the course command cheatsheet. The homework identifies the required outcomes; you must determine which commands produce them.

## Rules

- Work independently.
- Use only the supplied Homework 2 repository and your own new GitHub repository.
- Do not reinitialize the supplied repository.
- Work only on `main`; do not create another branch.
- Do not use merges, Pull Requests, conflict exercises, or recovery commands.
- Stage only the file required for each commit.
- Do not force push.
- Read and evaluate Git's output before continuing.

---

## Step 1 — Verify the starting repository

Open the extracted `CSC350_HW2_Independent_Repo` folder in VS Code.

Produce evidence that:

- the folder is already a Git repository;
- the current branch is `main`;
- the working tree is clean;
- the preparation commit `docs: prepare independent homework repository` is present;
- no remote repository is configured; and
- Git will use your correct name and email for new commits.

Record the requested starting evidence in `FESTIVAL_VISITOR_GUIDE.md`.

Stop and ask for help if the folder is not a Git repository or the starting working tree is not clean.

## Step 2 — Publish the starter repository

Create your own empty GitHub repository named:

```text
CSC350-HW2-YOUR-GITHUB-USERNAME
```

Do not initialize it with a README, `.gitignore`, or license.

Connect the supplied local repository to this GitHub repository and publish the existing `main` branch.

Required outcome:

- the GitHub repository displays all supplied homework files;
- the preparation commit appears on GitHub;
- the local `main` branch tracks the corresponding branch on GitHub; and
- `FESTIVAL_VISITOR_GUIDE.md` records your personal homework repository URL.

Stop before publishing if the configured remote URL does not identify your personal Homework 2 repository.

## Step 3 — Personalize the festival guide

Complete these sections of `FESTIVAL_VISITOR_GUIDE.md`:

- Student Information
- Repository Evidence
- Festival Identity
- Prediction Before the First Commit

Create an original festival name, location, intended audience, and one-sentence theme.

Before committing, use appropriate Git evidence to confirm:

- only the intended file changed;
- the saved changes are initially unstaged;
- the correct file is staged; and
- the staged snapshot contains only the intended changes.

Create and publish one focused commit with this exact message:

```text
docs: personalize festival visitor guide
```

Record its short commit ID in the evidence table and verify that the commit appears on GitHub.

## Step 4 — Add visitor access information

Complete these sections:

- Arrival Information
- Accessibility Information
- Visitor Reminder

Your guide must contain:

- one public-transit or parking instruction;
- one specific entrance or meeting location;
- two concrete accessibility provisions; and
- one concise safety or visitor reminder.

Use the same inspect → stage → verify → commit process practiced in Lab 1.

Create and publish one focused commit with this exact message:

```text
docs: add visitor access information
```

Record its short commit ID and verify the published content on GitHub.

## Step 5 — Demonstrate an update created on GitHub

First, produce evidence that your local working tree is clean.

Using GitHub's web editor, replace the placeholder in the **GitHub Verification** section with:

```text
Verified on GitHub by YOUR NAME.
```

Create the GitHub-side commit with this exact message:

```text
docs: verify independent homework on GitHub
```

Required outcome:

- before synchronization, the new commit and sentence exist on GitHub but not in your local copy;
- after synchronization, the local repository contains the GitHub-created commit;
- the verification sentence appears in the local file; and
- the same short commit ID is visible locally and on GitHub.

Record that commit ID in the evidence table. Do not create a second commit for the same verification sentence.

## Step 6 — Complete the reflection

Answer all five questions in the **Individual Reflection** section using one or two complete sentences per answer.

Inspect and stage only the reflection changes. Create and publish one focused commit with this exact message:

```text
docs: complete independent Git reflection
```

Record its short commit ID.

## Final required state

Produce evidence that:

- all placeholders in `FESTIVAL_VISITOR_GUIDE.md` have been replaced;
- the four required student commits appear in the correct order;
- the working tree is clean;
- local `main` and its GitHub branch are synchronized;
- the newest local and GitHub commit IDs match; and
- the completed guide is visible in your personal Homework 2 GitHub repository.

Use `SUBMISSION-CHECKLIST.md` to review your work.

## Submit

Submit only the URL of your personal `CSC350-HW2-YOUR-GITHUB-USERNAME` repository through the course system.

Do not submit the pair repository used for Activities 03–08.
