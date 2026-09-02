# Technocore Setup Guide for Windows

This guide provides a beginner-friendly overview of setting up a development environment for Technocore-related projects on Windows.

## Requirements

A basic Windows development environment may include:

* Windows 10 or Windows 11
* PowerShell
* Git
* Node.js
* A GitHub account
* A secure location for private credentials

## 1. Check PowerShell

Open Windows PowerShell and run:

```powershell
$PSVersionTable.PSVersion
```

This displays the installed PowerShell version.

## 2. Check Git

Run:

```powershell
git --version
```

If Git is installed, the command will display the installed version.

## 3. Check Node.js

Run:

```powershell
node --version
```

You can also check npm:

```powershell
npm --version
```

## 4. Clone a Repository

To clone a GitHub repository:

```powershell
git clone https://github.com/USERNAME/REPOSITORY.git
```

Replace `USERNAME` and `REPOSITORY` with the appropriate GitHub repository.

Then enter the repository:

```powershell
cd REPOSITORY
```

## 5. Basic Git Workflow

After making changes to a project:

```powershell
git status
git add .
git commit -m "Describe the change"
git push
```

A simple workflow is:

```text
Edit Files
    ↓
git status
    ↓
git add
    ↓
git commit
    ↓
git push
```

## 6. Protect Your Credentials

Never store private credentials directly in a public repository.

Avoid committing files containing:

```text
.env
.env.local
private keys
seed phrases
passwords
API secrets
```

A `.gitignore` file can help prevent accidental commits.

Example:

```gitignore
.env
.env.local
*.key
*.pem
secrets/
```

## 7. Verify Before Publishing

Before pushing changes to GitHub, review the files that will be committed:

```powershell
git status
```

You can also inspect the changes:

```powershell
git diff
```

Make sure sensitive information is not included.

## Conclusion

Windows provides a practical environment for learning Git, GitHub, decentralized identity, and AI-agent development.

Always keep private credentials secure and publish only information that is intended to be public.
