# Experiment 01 — Git setup and local version control

**Student:** [Your name]  
**Register number:** [Your register number]  
**Course:** Collaborative Development and DevOps

## Aim

Configure Git, create a local repository, record a change, and inspect the resulting commit history.

## Requirements

- Git installed: check with `git --version`.
- A terminal (PowerShell, Command Prompt, or a Unix shell).

## Procedure

1. Set the author information used in commits. Replace the sample values with your own:
   ```sh
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git config --global --list
   ```
2. Create a working folder and initialize Git:
   ```sh
   mkdir git-basics-lab
   cd git-basics-lab
   git init
   git status
   ```
3. Add a small file:
   ```sh
   printf "My first tracked file.\n" > notes.txt
   git status
   git add notes.txt
   git status
   ```
4. Save the staged change as a commit and inspect it:
   ```sh
   git commit -m "Add first lab note"
   git log --oneline
   git show --stat --oneline HEAD
   ```
5. Change the file, then compare the working tree with the committed version:
   ```sh
   printf "A second line.\n" >> notes.txt
   git diff
   git status
   ```

## What to record

Capture the output of `git --version`, `git status` before and after staging, and `git log --oneline`. Explain the difference between a modified file, a staged change, and a commit.

## Result

Complete this section after performing the commands. Do not report output you did not observe.

## Reference and attribution

The reference repository [DevOps_LAB_01](https://github.com/Smirk1308/DevOps_LAB_01) contained course/student metadata but no experiment instructions or implementation. This exercise is independently authored as an introductory Git lab.