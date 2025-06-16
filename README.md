# GitHub Actions Automatic Commits Demo

A just-for-fun demonstration of how to set up automatic commits using GitHub Actions.

## What is this?

This repository is a simple example showcasing how you can configure GitHub Actions to automatically commit changes to your repository.  It's not intended to be a practical tool, but rather an illustration of the capabilities of GitHub Actions.

**Disclaimer:** Automatically committing to your repository should be done with caution.  Ensure you understand the implications before setting up such a workflow in a real project.  This is a *demonstration*, not a best practice for most use cases.

## How it works

The workflow is defined in `.github/workflows/auto-commit.yml`.  It does the following:

1.  **Triggers:** The workflow is triggered by a push to the `master` branch, and also on a schedule.
2.  **Checkout:** The workflow checks out the repository's code.
3.  **Make Changes:** The workflow modifies the `LAST_UPDATED` file (in this case, by updating the timestamp).
4.  **Commit:** The workflow commits the changes.
5.  **Push:** The workflow pushes the commit back to the `master` branch.
