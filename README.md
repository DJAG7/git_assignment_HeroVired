# Hero Vired Git and Github Assignment

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

### 4. Push the code to the dev branch and V1 release
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

  ### 4. Push the code to the dev branch and V1 release
```bash
git checkout main
git merge dev
git tag -a v1.0 -m "V1"
git push origin main --tags

```

# Geometry Calculator

This repository contains a simple Python program that calculates the area of a circle and the area of a rectangle. Additionally, it demonstrates the integration of Git LFS (Large File Storage) to handle large binary files efficiently.

## Geometry Calculator Steps:

### Feature Development Workflow:

1. **Create a New Branch and Push Initial File (Circle Area):**
    ```bash
    git checkout main
    git checkout -b feature/circle-area
    git add geometrycalculator.py
    git commit -m "Initial commit: geometrycalculator.py"
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
    git commit -m "Implement circle area feature"
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
    git commit -m "Implement rectangle area feature"
    git push origin feature/rectangle-area
    ```

### Pull Requests and Merging:

9. **Create Pull Requests:**
    - Create pull requests for both branches targeting the 'geometry-calculator' branch on your Git hosting platform.

10. **Review and Merge:**
    - Have another team member or reviewer review your pull requests.
    - After receiving approval, merge both pull requests into the 'geometry-calculator' branch.

---

# Git LFS Integration

This repository demonstrates the integration of Git LFS (Large File Storage) to efficiently handle large binary files. A large binary file (`large_file.bin`) was added, committed, and pushed to the repository.

## Git LFS Steps:

1. **Initialize Git LFS:**
    ```bash
    git lfs install
    git lfs track "*.bin"
    git add .gitattributes
    git commit -m "Initialize Git LFS"
    ```

2. **Commit and Push Large Binary File:**
    ```bash
    git add large_file.bin
    git commit -m "Add large binary file using Git LFS"
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

---

Feel free to customize this README based on your specific project details and add any additional sections or details you find relevant.
