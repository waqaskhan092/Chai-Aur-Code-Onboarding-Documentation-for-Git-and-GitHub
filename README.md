# Chai aur Code - Onboarding Documentation for Git and GitHub

## Introduction

Welcome to the ChaiCode Web Dev Cohort! As a developer here, you'll rely heavily on Git and GitHub for version control and team collaboration. This guide will help you get started with Git and GitHub, ensuring a smooth onboarding experience. By the end of this document, you'll understand how to set up Git, use essential commands, and follow ChaiCode's workflows for seamless teamwork.

---

## Basics of Git and GitHub

### Git vs. GitHub: What's the Difference?

#### What is Git?

Git is a version control system used to track changes in your files. It’s free, open-source software that you can install on Windows, macOS, and Linux. Think of Git as software that works locally on your computer to manage your project's history.

#### What is GitHub?

GitHub, on the other hand, is a web-based hosting service for Git repositories. It’s an online platform that allows you to store, share, and collaborate on code with others. While GitHub is one of the most popular platforms for hosting Git repositories, it’s not the only one—others include GitLab and Bitbucket.

### Basics About Version Control Systems

Version control systems (VCS) manage the history of your code. They allow you to track changes, collaborate with others, and revert to earlier versions of your files when needed. Imagine version control as checkpoints in a game—you can save your progress, go back to an earlier checkpoint, or branch off to explore a new path. In software development, this ensures your code is always recoverable and manageable.

Before Git became popular, developers used proprietary systems like SCCS (Source Code Control System). These were often expensive and less user-friendly. Git was created to make version control more accessible and powerful. Other examples of VCS include Subversion (SVN), CVS, and Perforce.

---

## Installation and Setup

### Step 1: Install Git

#### Windows:

1. Download the Git installer from <a href="https://git-scm.com/" target="_blank">git-scm.com</a>.
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

If you don’t have a GitHub account, sign up at <a href="https://github.com/" target="_blank">github.com</a>.

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

Good luck!
