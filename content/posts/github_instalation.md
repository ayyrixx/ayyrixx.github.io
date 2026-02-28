+++
date = '2026-02-28T16:00:00+05:00'
title = 'Instalation Guide for windows and Linux (Arch)'
+++
# Installing Git and GitHub Setup

This guide explains how to install **Git** and connect it with your GitHub account on:

* Windows
* Arch Linux

---

# 🪟 Windows Installation Guide

## 1️⃣ Download Git

1. Open your browser.
2. Go to: [https://git-scm.com/download/win](https://git-scm.com/download/win)
3. Download the installer.
4. Run the `.exe` file.

## 2️⃣ Install Git

During installation:

* Keep default settings.
* Click **Next** until installation finishes.
* Click **Finish**.

## 3️⃣ Verify Installation

Open **Command Prompt** or **PowerShell** and run:

```bash
git --version
```

If installed correctly, it will show the Git version.

## 4️⃣ Configure Git

Set your name and email (use your GitHub email):

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

Check configuration:

```bash
git config --list
```

---

# 🐧 Arch Linux Installation Guide

## 1️⃣ Install Git

Open terminal and run:

```bash
sudo pacman -S git
```

Press `Y` to confirm installation.

## 2️⃣ Verify Installation

```bash
git --version
```

## 3️⃣ Configure Git

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

Verify:

```bash
git config --list
```

---

# 🔐 Connect Git to GitHub (SSH Method – Recommended)

## 1️⃣ Generate SSH Key

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Press Enter for default location.

## 2️⃣ Start SSH Agent

### Windows (PowerShell):

```bash
Start-Service ssh-agent
ssh-add $env:USERPROFILE\.ssh\id_ed25519
```

### Arch Linux:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

## 3️⃣ Copy SSH Key

### Windows:

```bash
type $env:USERPROFILE\.ssh\id_ed25519.pub
```

### Arch Linux:

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the output.

## 4️⃣ Add SSH Key to GitHub

1. Go to GitHub.
2. Open **Settings**.
3. Go to **SSH and GPG keys**.
4. Click **New SSH key**.
5. Paste your key.
6. Click **Add SSH key**.

## 5️⃣ Test Connection

```bash
ssh -T git@github.com
```

If successful, you will see a welcome message.

---

# ✅ Clone a Repository

```bash
git clone git@github.com:username/repository.git
```

---

# ✅ Basic Git Commands

```bash
git status
git add .
git commit -m "Initial commit"
git push
```

---

# 🎯 Installation Complete

You now have Git installed and connected to GitHub on Windows or Arch Linux.
