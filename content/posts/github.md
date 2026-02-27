+++
date = '2026-02-26T16:00:00+05:00'
title = 'Setting Up GitHub on Linux and Pushing Code'
draft = false
+++

In this post, I explain how I set up GitHub on my Linux system and pushed my code step by step.

---

## Step 1: Install Git

First, install Git:

```bash
sudo pacman -S git
```

Verify installation:

```bash
git --version
```

---

## Step 2: Configure Git

Set your username and email:

```bash
git config --global user.name "ayyrixx"
git config --global user.email "aliyanniazi374@gmail.com"
```

Check configuration:

```bash
git config --list
```

---

## Step 3: Create a Repository on GitHub

1. Login to GitHub
2. Click **New Repository**
3. Enter repository name
4. Click **Create Repository**

---

## Step 4: Initialize Local Project

Go to your project folder and run:

```bash
git init
```

Add files:

```bash
git add .
```

Commit files:

```bash
git commit -m "Initial commit"
```

---

## Step 5: Connect Local Repository to GitHub

Copy your repository URL from GitHub and run:

```bash
git remote add origin https://github.com/ayyrixx/repository-name.git
```

Verify remote:

```bash
git remote -v
```

---

## Step 6: Push Code to GitHub

```bash
git branch -M main
git push -u origin main
```

Now your project is successfully uploaded.

---

## Step 7: Updating Code Later

Whenever you make changes:

```bash
git add .
git commit -m "Updated project"
git push
```

---

## Conclusion

Setting up GitHub on Linux involves:

* Installing Git
* Configuring user details
* Initializing repository
* Connecting to GitHub
* Pushing code

With this workflow, I can now manage and track all my projects efficiently.
