# Chai aur Code Onboarding Documentation for Git and GitHub


# Welcome to Git and GitHub at ChaiCode Cohort!

## Introduction
Welcome to the ChaiCode Cohort! As a developer here, you'll rely heavily on Git and GitHub for version control and team collaboration. This guide will help you get started with Git and GitHub, ensuring a smooth onboarding experience. By the end of this document, you'll understand how to set up Git, use essential commands, and follow ChaiCode's workflows for seamless teamwork.

---

## Basics of Git and GitHub

### What is Git?
Git is a distributed version control system that allows developers to track changes in their code, collaborate with others, and manage multiple versions of a project efficiently. It is an essential tool for modern software development.

### What is GitHub?
GitHub is a web-based platform built on top of Git. It provides a centralized space for hosting repositories, collaborating with team members, reviewing code, and managing projects. GitHub makes teamwork easier and ensures that everyone is on the same page.

---

## Installation and Setup

### Step 1: Install Git

#### Windows:
1. Download the Git installer from [git-scm.com](https://git-scm.com/).
2. Run the installer and follow the prompts.
3. Verify the installation by opening a terminal and running:
   ```bash
   git --version
   ```

#### macOS:
1. Open Terminal and install Git using Homebrew:
   ```bash
   brew install git
   ```
2. Verify the installation:
   ```bash
   git --version
   ```

#### Linux:
1. Use your package manager to install Git:
   ```bash
   sudo apt update
   sudo apt install git
   ```
2. Verify the installation:
   ```bash
   git --version
   ```

### Step 2: Configure Git
Set your username and email globally:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 3: Create a GitHub Account
If you don’t have a GitHub account, sign up at [github.com](https://github.com/).

---

## Cloning the ChaiCode Repository
1. Navigate to the GitHub repository page.
2. Copy the repository URL.
3. Run the following command in your terminal:
   ```bash
   git clone https://github.com/ChaiCode/example-repo.git
   ```
4. Navigate into the cloned repository folder:
   ```bash
   cd example-repo
   ```

---

## Basic Git Commands

### Common Commands
- **Check the status of your repository:**
  ```bash
  git status
  ```
- **Stage changes:**
  ```bash
  git add <file-name>
  ```
- **Commit changes with a message:**
  ```bash
  git commit -m "Your commit message"
  ```
- **Push changes to GitHub:**
  ```bash
  git push
  ```
- **Pull updates from GitHub:**
  ```bash
  git pull
  ```
- **View commit history:**
  ```bash
  git log
  ```

### Screenshots
Screenshots of these commands being executed are provided in the repository for reference.

---

## Commit Message Rules
1. Use the present tense (e.g., "Add feature" not "Added feature").
2. Capitalize the first letter of the message.
3. Keep the message short (50 characters or less).
4. Use prefixes like `fix:`, `feat:`, `chore:`, or `docs:`.

### Examples
- `feat: Add tea selection feature`
- `fix: Resolve login issue for tea enthusiasts`
- `docs: Update README with chai varieties`

---

## Branching Workflow

### Branch Strategy
At ChaiCode, we use the following branching strategy:
- `main`: Production-ready code.
- `development`: In-progress features.
- `feature/<name>`: Individual features.

### Create and Switch Branches
- Create a new branch:
  ```bash
  git branch feature/tea-menu
  ```
- Switch to the branch:
  ```bash
  git checkout feature/tea-menu
  ```

### Merging and Resolving Conflicts
1. Merge your branch into `development` once your feature is complete.
   ```bash
   git checkout development
   git merge feature/tea-menu
   ```
2. Resolve any conflicts in the code editor and commit the changes.

---

## Pull Requests (PR)
1. Push your branch to GitHub:
   ```bash
   git push -u origin feature/tea-menu
   ```
2. Navigate to the GitHub repository.
3. Click **Pull Request** and select your branch.
4. Write a descriptive title and summary for your PR.
5. Request a review from a team member and submit the PR.

---

## Best Practices
1. Commit regularly and meaningfully.
2. Use descriptive commit messages.
3. Pull updates frequently to minimize conflicts.

---

## Deliverables
Your repository should include:
1. A formatted `README.md` file with embedded screenshots.
2. At least 5 meaningful commits.
3. A sample branch created and merged with `main`.
4. At least one pull request demonstrating the workflow.

Good luck, and welcome to ChaiCode!

