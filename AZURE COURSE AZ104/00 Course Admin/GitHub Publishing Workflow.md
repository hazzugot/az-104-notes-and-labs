---
course: AZ-104
title: GitHub Publishing Workflow
type: admin
updated: 2026-09-17
tags:
  - az104
  - github
  - portfolio
  - linkedin
---

# GitHub Publishing Workflow

Use this when publishing the AZ-104 vault as a GitHub portfolio repo and then sharing it on LinkedIn.

**Index:** [[AZ-104 Course Index]]

---

## Publishing Goal

Turn the vault into a public learning-evidence repo:

- Course notes show the concepts learned.
- Lab notes show hands-on Azure portal practice.
- Screenshots prove practical work without exposing private account details.
- The exam tracker shows what is complete and what still needs revision.

---

## Pre-Publish Checklist

### 1. Check for private information

Search the vault before publishing:

```bash
rg -n "subscription|tenant|client secret|password|key|token|sas|shared access|@|[0-9]{1,3}(\\.[0-9]{1,3}){3}" .
```

Manually inspect screenshots in `_attachments/` for:

- subscription IDs
- tenant IDs
- personal email addresses
- public IP addresses
- storage access keys
- SAS tokens
- resource names you do not want public

If a screenshot exposes anything sensitive, redact it before pushing.

### 2. Check Markdown links

From the vault root:

```bash
find . -name "*.md" -print
```

Open the vault in Obsidian and check the graph or unresolved links view. Fix missing links before publishing.

### 3. Keep local Obsidian state out of Git

The repo includes a `.gitignore` that excludes volatile Obsidian workspace state and common secret formats. Keep `.obsidian/workspace.json` private because it only records your local editor layout.

---

## First GitHub Upload

Run these commands from the vault root:

```bash
git init
git add README.md .gitignore "AZURE COURSE AZ104"
git status
git commit -m "Publish AZ-104 course notes and labs"
```

Create a new GitHub repository named something like:

```text
az-104-notes-and-labs
```

Then connect and push:

```bash
git branch -M main
git remote add origin git@github.com:YOUR-USERNAME/az-104-notes-and-labs.git
git push -u origin main
```

If using HTTPS instead of SSH:

```bash
git remote add origin https://github.com/YOUR-USERNAME/az-104-notes-and-labs.git
git push -u origin main
```

---

## Suggested Commit Flow

Use small commits as the notes improve:

```bash
git status
git add "AZURE COURSE AZ104"
git commit -m "Refine AZ-104 networking revision notes"
git push
```

Good future commit topics:

- Add endpoint revision notes.
- Finish ARM and Bicep hands-on objectives.
- Add blob versioning lab notes.
- Add App Service backup notes.
- Add VM move notes.
- Convert recall checks into flashcards.

---

## LinkedIn Posting Workflow

1. Push the repo to GitHub.
2. Open the GitHub repo page and check that the README renders properly.
3. Open the course index from GitHub and make sure links work well enough for a public reader.
4. Copy the GitHub repo URL.
5. Use [[LinkedIn Post Draft - AZ-104 Notes and Labs]] as the starting post.
6. Add 2-4 screenshots to the LinkedIn post:
   - course index or exam tracker
   - one networking lab screenshot
   - one monitoring or backup screenshot
   - one Azure portal evidence screenshot
7. Keep the post focused on what you learned, what you built, and what you are revising next.

---

## GitHub Repo Description

```text
AZ-104 Microsoft Azure Administrator course notes, hands-on labs, screenshots, and revision tracker.
```

## Suggested Topics

```text
azure az-104 microsoft-azure cloud-computing sysadmin networking storage monitoring devops learning-notes
```

## Suggested LinkedIn Hashtags

```text
#Azure #MicrosoftAzure #AZ104 #CloudComputing #AzureAdministrator #LearningInPublic
```
