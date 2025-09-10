# 🌿 What is a Branch in Git?

A **branch** in Git is like a **parallel line of development**.  
It lets you work on new features, bug fixes, or experiments without disturbing the main project.

---

## 🔑 Key Points

1. **Pointer to a Commit**
   - A branch is essentially a lightweight **pointer to a specific commit**.
   - The default branch in Git is usually called `main` (earlier `master`).

2. **Isolation**
   - You can make changes in a branch without affecting the main codebase.
   - This avoids breaking production code while experimenting.

3. **Collaboration**
   - Each developer can create their own branch for a feature.
   - Later, branches are merged back into the main branch.

4. **Workflow**
   - Branches are used in workflows like:
     - **Feature Branching** → one branch per feature.
     - **Release Branching** → one branch per release.
     - **Hotfix Branching** → quick fixes for urgent bugs.

---

## 🖥️ Example

```bash
# Create a new branch
git branch feature-login

# Switch to the branch
git checkout feature-login
# or modern way
git switch feature-login

# Work on changes...
git add .
git commit -m "Added login feature"

# Merge branch back to main
git checkout main
git merge feature-login
```

---

## 📊 Visual Example

```
main:    A --- B --- C
                 \
feature-login:     D --- E
```

- `A, B, C` = commits on the main branch  
- `D, E` = commits on the feature branch  

When merged, they combine back into one history.

---

## 👉 In Short
A **branch = a separate workspace** inside Git that helps you manage multiple versions of your project simultaneously.
