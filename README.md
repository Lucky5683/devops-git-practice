# DevOps Project 
# DevOps Git Project

## Objective
Manage a DevOps project using Git and GitHub best practices.

## Branching Strategy
- **main**: Stable, production-ready code
- **dev**: Integration branch
- **feature/***: Used for feature development

## Project Structure
- `scripts/` - Bash scripts or deployment tools
- `docs/` - Project documentation

## How to Contribute
1. Create a feature branch
2. Make changes
3. Push and raise a Pull Request
## Contributors
- Dinesh (Lucky5683)
 

#code
# DevOps Git Project - Workflow Summary

## Git Workflow Steps Performed

```bash
# Initialize local Git repo (already done)
git init

# Add files and commit initial version
git add .
git commit -m "Initial commit with README and .gitignore"

# Add GitHub remote repo (if not already added)
git remote add origin https://github.com/Lucky5683/devops-git-practice.git
# Or update remote URL if already exists
git remote set-url origin https://github.com/Lucky5683/devops-git-practice.git

# Rename local branch to main
git branch -M main

# Push local main branch to GitHub
git push -u origin main

# Create and switch to dev branch
git checkout -b dev
git push -u origin dev

# Create and switch to feature branch (example: feature/readme-update)
git checkout -b feature/readme-update
git push -u origin feature/readme-update

# Make changes to README.md (manually edited)

# Stage and commit changes on feature branch
git add README.md
git commit -m "Add contributor section"
git push

# (On GitHub) Create Pull Request: feature/readme-update -> dev and merge

# Back locally, switch to dev branch and pull latest changes
git checkout dev
git pull origin dev

# Push dev branch (optional if any local commits)
git push origin dev

# (On GitHub) Create Pull Request: dev -> main and merge

# Update local main branch with latest changes
git checkout main
git pull origin main

---

### Step 3: Save and close Notepad

---

### Step 4: Stage, commit, and push to `main`

```bash
git add README.md
git commit -m "Add Git workflow summary to README"
git push origin main

