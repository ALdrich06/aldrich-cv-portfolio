# GitHub Merge Conflict Simulation - Activity Report

**Student Name:** Aldrich A. Alimpolos  
**Year Level:** 4th Year  
**Set/Section:** BSIT 4D  
**Subject:** IT415  
**Activity:** Module 2 – Lesson 3–4, Slide 18 - Merge Conflict Simulation  
**Date:** September 29, 2026

---

## Repository Information
- **Repository URL:** https://github.com/ALdrich06/aldrich-cv-portfolio
- **File Modified:** README.md
- **Branches Created:** branch-a, branch-b

---

## Step-by-Step Process

### Step 1: Initial Setup
**Action:** Cloned the existing GitHub repository to local machine

**Commands Used:**
```bash
git clone https://github.com/ALdrich06/aldrich-cv-portfolio.git
cd aldrich-cv-portfolio
git status
```

**Result:** Successfully cloned repository with 2 existing commits on main branch

---

### Step 2: Create Branch-A
**Action:** Created first branch and made modifications to README.md

**Commands Used:**
```bash
git checkout -b branch-a
git branch
```

**Changes Made in Branch-A:**
- Modified the "About This Project" section
- Added: **Project Status:** Completed
- Added: **Last Updated:** September 2026
- Expanded Technologies Used list:
  - Added JavaScript
  - Added Bootstrap Framework

**Commit Command:**
```bash
git add README.md
git commit -m "Branch-A: Add project status and expand technologies list"
```

**Commit Hash:** 55367f4

---

### Step 3: Create Branch-B
**Action:** Switched back to main branch and created second branch with DIFFERENT changes to the SAME section

**Commands Used:**
```bash
git checkout main
git checkout -b branch-b
git branch
```

**Changes Made in Branch-B:**
- Modified the SAME "About This Project" section
- Added: **Development Phase:** In Progress
- Added: **Version:** 1.0
- Modified Technologies Used list:
  - Added CSS3 (with Flexbox)
  - Added Responsive Web Design

**Commit Command:**
```bash
git add README.md
git commit -m "Branch-B: Add development phase and update CSS description"
```

**Commit Hash:** 6607950

---

### Step 4: Intentionally Create Merge Conflict
**Action:** Attempted to merge branch-a into branch-b

**Command Used:**
```bash
git merge branch-a
```

**Result:** MERGE CONFLICT DETECTED!

**Git Output:**
```
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
```

**Status Check:**
```bash
git status
```

**Output:**
```
On branch branch-b
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   README.md
```

---

### Step 5: Examine the Conflict
**Action:** Viewed the conflicting file to see conflict markers

**Conflict Markers in README.md:**
```markdown
## About This Project
This repository contains my personal CV webpage created as a requirement for IT415. The webpage showcases my educational background, skills, and contact information in a professional and responsive design.

<<<<<<< HEAD
**Development Phase:** In Progress  
**Version:** 1.0

## Technologies Used
- HTML5
- CSS3 (with Flexbox)
- Responsive Web Design
=======
**Project Status:** Completed  
**Last Updated:** September 2026

## Technologies Used
- HTML5
- CSS3
- JavaScript
- Bootstrap Framework
>>>>>>> branch-a
- GitHub Pages
```

**Explanation of Conflict Markers:**
- `<<<<<<< HEAD` - Marks the beginning of current branch (branch-b) changes
- `=======` - Separates the two conflicting versions
- `>>>>>>> branch-a` - Marks the end and shows the incoming branch name

---

### Step 6: Resolve the Conflict
**Action:** Manually edited the file to combine the best parts from both branches

**Resolution Strategy:** 
Combined both sets of changes to create a comprehensive version that includes:
- All metadata from both branches
- All technologies from both branches
- Removed all conflict markers

**Resolved Content:**
```markdown
## About This Project
This repository contains my personal CV webpage created as a requirement for IT415. The webpage showcases my educational background, skills, and contact information in a professional and responsive design.

**Project Status:** Completed  
**Version:** 1.0  
**Last Updated:** September 2026

## Technologies Used
- HTML5
- CSS3 (with Flexbox)
- JavaScript
- Bootstrap Framework
- Responsive Web Design
- GitHub Pages
```

---

### Step 7: Commit the Resolved Conflict
**Action:** Staged and committed the resolved file

**Commands Used:**
```bash
git add README.md
git status
git commit -m "Resolve merge conflict: Combine project info from both branches"
```

**Result:** Merge conflict successfully resolved!

**Commit Hash:** f5d3fc1

---

### Step 8: Merge to Main Branch
**Action:** Merged the resolved branch-b into main branch

**Commands Used:**
```bash
git checkout main
git merge branch-b
```

**Result:** Fast-forward merge successful (no conflicts because branch-b already contains the resolved changes)

---

### Step 9: Push to GitHub
**Action:** Pushed all changes and branches to GitHub repository

**Commands Used:**
```bash
git push origin main
git push origin branch-a
git push origin branch-b
```

**Result:** All branches successfully pushed to GitHub!

---

## Final Git Log Graph

```
*   f5d3fc1 Resolve merge conflict: Combine project info from both branches
|\  
| * 55367f4 Branch-A: Add project status and expand technologies list
* | 6607950 Branch-B: Add development phase and update CSS description
|/  
* a168766 Updated personal information and added more details
* fa99f17 Initial commit: Added CV webpage and README
```

---

## Summary of Deliverables

### ✅ Branches Used
1. **main** - Original branch
2. **branch-a** - First feature branch with project status updates
3. **branch-b** - Second feature branch with development phase info

### ✅ Conflicting Changes
- **Branch-A Changes:**
  - Project Status: Completed
  - Last Updated: September 2026
  - Added: JavaScript, Bootstrap Framework

- **Branch-B Changes:**
  - Development Phase: In Progress
  - Version: 1.0
  - Added: CSS3 (with Flexbox), Responsive Web Design

### ✅ Merge Conflict Encountered
- File: README.md
- Lines affected: "About This Project" section and "Technologies Used" section
- Conflict markers: `<<<<<<< HEAD`, `=======`, `>>>>>>> branch-a`

### ✅ Conflict Resolution
- Strategy: Combined all useful information from both branches
- Removed all conflict markers
- Created a comprehensive version with all technologies and metadata

### ✅ Final Successful Merge
- Resolved commit: f5d3fc1
- Merged into main branch
- All branches pushed to GitHub

### ✅ Updated GitHub Repository
- Repository URL: https://github.com/ALdrich06/aldrich-cv-portfolio
- All branches visible on GitHub
- Commit history shows merge conflict resolution

---

## Key Learning Points

1. **Branch Creation:** Successfully created separate branches from the same base commit
2. **Conflicting Changes:** Made different modifications to the same lines in the same file
3. **Merge Conflict Recognition:** Identified conflict markers and understood their meaning
4. **Conflict Resolution:** Manually resolved conflicts by combining changes appropriately
5. **Git Workflow:** Completed full workflow from branch creation to pushing resolved changes

---

## Commands Reference

### Essential Commands Used:
```bash
# Clone repository
git clone <repository-url>

# Create and switch to new branch
git checkout -b <branch-name>

# View branches
git branch

# Stage changes
git add <file>

# Commit changes
git commit -m "message"

# Merge branches
git merge <branch-name>

# Check status
git status

# View log with graph
git log --oneline --all --graph

# Push to GitHub
git push origin <branch-name>
```

---

## Conclusion

This activity successfully demonstrated the complete process of creating, encountering, and resolving a merge conflict in Git. The simulation followed the procedure outlined in Module 2 – Lesson 3–4, Slide 18, and all deliverables have been completed and pushed to the GitHub repository.

**Repository Evidence:** All changes are visible at https://github.com/ALdrich06/aldrich-cv-portfolio

---

**Prepared by:** Aldrich A. Alimpolos  
**Date:** September 29, 2026
