# Hero Vired Git and Github Assignment
-Reviewing was done by Janisha, @janisha42 
# CalculatorPlus

Simple calculator to perform basic math operations (+-*/). Also adding square root as another feature.

### 1. Create a Repository:

- Create a new repository named `git_assignment_HeroVired`.

### 2. Clone the Repository and Create a Main and Development Branch:

```bash
git clone <repository_url>
cd git_assignment_HeroVired
git checkout -b main
git checkout -b dev
```

### 3. Push the code to the dev branch and V1 release
```bash
git checkout main
git merge dev
git tag -a v1.0 -m "V1"
git push origin main --tags
```

## Steps to Add Square Root Functionality:

- Add the code in the python file.
- Push the python file via feature/sqrt branch
- Merge the Branch with the main branch

```bash

git checkout -b feature/sqrt
git add geometrycalculator.py
git commit -m "Implement square root feature and fix divide bug"
git push origin feature/sqrt
```

# Geometry Calculator

Program to Calculate Circle and Rectangular Area

## Geometry Calculator Steps:



1. **Create a New Branch and Push Initial File (Circle Area):**
    ```bash
    git checkout main
    git checkout -b feature/circle-area
    git add geometrycalculator.py
    git commit -m "Commit 1"
    git push origin feature/circle-area
    ```

2. **Stash Changes for Circle Area Feature:**
    ```bash
    git stash
    git status
    ```

3. **Create a New Branch for Rectangle Area Feature:**
    ```bash
    git checkout -b feature/rectangle-area
    ```

4. **Stash Changes for Rectangle Area Feature:**
    ```bash
    git stash
    git status
    ```

5. **Switch Back to Circle Area Branch:**
    ```bash
    git checkout feature/circle-area
    git stash apply
    ```

6. **Complete and Push Circle Area Feature:**
    ```bash
    git add .
    git commit -m "Implementing circle area feature"
    git push origin feature/circle-area
    ```

7. **Switch Back to Rectangle Area Branch:**
    ```bash
    git checkout feature/rectangle-area
    git stash apply
    ```

8. **Complete and Push Rectangle Area Feature:**
    ```bash
    git add .
    git commit -m "Implementing rectangle area feature"
    git push origin feature/rectangle-area
    ```

9. **Review and Merging**
  -Reviewing was done by Janisha, @janisha42 and then merged.
---

# Git LFS 

A large binary file was added to the repository using LFS integration

## Git LFS Steps:

1. **Initialize Git LFS:**
    ```bash
    git lfs install
    git lfs track "*.bin"
    git add .gitattributes
    git commit -m "LFS"
    ```

2. **Commit and Push Large Binary File:**
    ```bash
    git add 1GB.bin
    git commit -m "Adding 1GB File"
    git push origin main
    ```

3. **Clone Repository on Another Machine:**
    ```bash
    git clone <repository_url>
    cd git_assignment_HeroVired
    ```

4. **Verify Binary File Download:**
    ```bash
    git checkout main
    ```


