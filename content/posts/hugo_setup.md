---

title: "How I Built My Hugo Blog on Arch Linux"
date: 2026-02-27
draft: false
description: "A step-by-step explanation of how I created and deployed my Hugo blog."
tags: ["hugo", "arch-linux", "blogging", "static-site"]
categories: ["Tech"]
--------------------

## Introduction

In this post, I explain how I created my blog using Hugo on Arch Linux and deployed it successfully.

---

## Step 1: Installing Hugo

I installed Hugo using pacman:

```bash
sudo pacman -S hugo
```

Then I verified the installation:

```bash
hugo version
```

---

## Step 2: Creating a New Hugo Site

```bash
hugo new site myblog
cd myblog
```

This created the basic Hugo project structure.

---

## Step 3: Adding a Theme

I added a theme and configured it inside the `hugo.toml` file.

---

## Step 4: Creating a New Post

```bash
hugo new posts/my-second-blog.md
```

Then I edited the generated file and added my content.

---

## Step 5: Running the Local Server

To preview the website locally:

```bash
hugo server
```

Then I opened:

```
http://localhost:1313
```

---

## Step 6: Building and Deploying

To generate the static files:

```bash
hugo
```

Then I pushed the changes to GitHub:

```bash
git add .
git commit -m "Added second blog post"
git push
```

---

## Conclusion

This is how I built and deployed my Hugo blog. In future posts, I will explore customization, themes, and performance optimization.
