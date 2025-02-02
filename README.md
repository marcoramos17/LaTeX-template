# LaTeX-template
<div align="center">
  <!-- GitHub Profile Shield -->
  <a href="https://github.com/marcoramos17">
    <img src="https://img.shields.io/badge/GitHub-Profile-black" alt="My GitHub Profile">
  </a>

  <!-- LaTeX Template Shield -->
  <a href="https://marcoramos17.github.io/LaTeX-template/">
    <img src="https://img.shields.io/badge/LaTeX%20Template-Preview-blue" alt="LaTeX Template Preview">
  </a>
</div>



# LaTeX Template Repository

Welcome to the LaTeX Template repository. This repository serves as a centralized template for creating and managing LaTeX documents efficiently, with support for customizable cover pages and project-specific branches.

---

## Document Information

### Affiliation:
*Example University*

### Project:
*Module/Project Name*

### Title:
*Document Title Here*

### Author(s):
*Marco Ramos - 10415201*

### Description:
This repository provides a well-structured template for LaTeX documents. Each branch represents a unique project, coursework, or document. The main branch contains the template and other shared resources, such as cover pages and images, which can be imported into specific branches.

---

## Workflow Guide

### **Working with the Main Branch**
The `main` branch contains shared resources such as:
- Main LaTeX file with key configurations
- Imported LaTeX files for different sections (found in the `texsource` directory)
- Cover page templates (found in the `coverpages` directory)
- Images (found in the `img` directory)

#### Key Actions:
- **Update the template (`main` branch):**
  ```bash
  git checkout main
  # Make updates to the template
  git add .
  git commit -m "Update shared resources"
  git push
  ```

- **Prepare the template for new documents:**
  The `main` branch should always have the latest version of shared resources ready to be pulled into new branches.

---

### **Creating a New Document/Branch**
To start working on a new LaTeX document:

1. **Create a new branch OR switch to an existing branch:**
   ```bash
   git checkout -b document-branch-name
   #OR
   git checkout document-branch-name
   ```
   - Branch naming format: `affiliation_project_document-name`. Ex: `COV_6006CEM_Train-Accidents`

2. **Edit and customize the document:**
   - Make changes to `main.tex` and other imported files, as necessary.
   - Compile the document and check outputs.

3. **Push the branch to the remote repository (optional):**
   ```bash
   git push
   ```

---

### **Keeping The Document Branch Updated**
If updates are made to the template in the `main` branch, pull those changes into other document branches:

1. **Switch to another document branch:**
   ```bash
   git checkout document-branch-name
   ```

2. **Pull changes from `main`:**
   ```bash
   git pull origin main
   ```

3. **Resolve any merge conflicts (if applicable):**
   Open conflicting files, resolve issues manually, and mark them resolved:
   ```bash
   git add resolved-file.tex
   git commit
   ```

---

### **General Tips**
- Regularly pull updates from `main` to keep branches up-to-date with the latest template changes.
- Use descriptive branch names (e.g., `COV_6006CEM_Train-Accidents`).
- Write clear commit messages for better collaboration and tracking.

---

This README serves as an introduction to maintain an organized and efficient workflow for managing LaTeX documents.