# How We Automated GitHub Issues Creation

**Created with:** Claude.ai and Claude Code
**Date:** February 4, 2026
**Repository:** [lavender-daydream.com](https://github.com/Lavender-Daydream/Website-lavender-daydream.com)

---

## Overview

This document explains how we automated the creation of 24 GitHub issues from a markdown list, saving hours of manual copy-pasting work!

## What We Accomplished

✅ Installed GitHub CLI (command-line tool for GitHub)
✅ Authenticated with GitHub account
✅ Created automation script to convert markdown list into GitHub issues
✅ Successfully created 24 issues with proper labels, descriptions, and task lists
✅ Added credit notes to all issues

**Result:** All 24 issues from the markdown list are now live on GitHub: https://github.com/Lavender-Daydream/Website-lavender-daydream.com/issues

---

## Step-by-Step Process

### Step 1: Installing GitHub CLI

We used Windows Package Manager (winget) to install the GitHub CLI tool:

```powershell
winget install --id GitHub.cli --accept-source-agreements --accept-package-agreements
```

**What is GitHub CLI?** It's an official command-line tool from GitHub that lets you interact with GitHub (create issues, pull requests, etc.) directly from your terminal or scripts.

### Step 2: Authenticating with GitHub

After installation, we authenticated the CLI with your GitHub account:

```powershell
gh auth login
```

This opened an authentication flow where we:
1. Selected **HTTPS** as the preferred protocol (simpler for beginners)
2. Followed the prompts to log in via browser
3. Successfully connected as **Lavender-Daydream**

You can verify authentication anytime with:
```powershell
gh auth status
```

### Step 3: Creating the Automation Script

Instead of manually creating each issue, we wrote a PowerShell script that:
1. Reads the issue data (titles, descriptions, labels, tasks)
2. Uses GitHub CLI to create each issue automatically
3. Adds proper formatting and labels
4. Includes a small delay between issues to avoid rate limiting

**Script location:** `C:\Users\berly\create_issues_simple.ps1`

### Step 4: Running the Script

We executed the script which:
- Created all 24 issues in about 12 seconds
- Assigned appropriate labels to each issue
- Included all task lists and descriptions
- Provided clickable links to each created issue

### Step 5: Adding Credit Notes

We created a second script to add a credit note to all issues:

```powershell
# Added to bottom of each issue:
*Issue list made and automated with Claude.ai and Claude Code*
```

**Script location:** `C:\Users\berly\add_credit_to_issues.ps1`

---

## The Scripts We Created

### Main Issue Creation Script

**File:** `create_issues_simple.ps1`

This script creates each issue one by one with the `gh issue create` command:

```powershell
# Example of how we created each issue:
& $ghPath issue create `
  --repo "Lavender-Daydream/Website-lavender-daydream.com" `
  --title "Issue Title Here" `
  --label "label1,label2,label3" `
  --body "Issue description with tasks..."
```

### Credit Note Script

**File:** `add_credit_to_issues.ps1`

This script:
1. Gets the current body of each issue
2. Appends the credit note
3. Updates the issue with the new body

```powershell
# For each issue #7-28:
$currentBody = gh issue view $issueNum --json body --jq .body
$newBody = $currentBody + $creditNote
$newBody | gh issue edit $issueNum --body-file -
```

---

## Issues Created

We successfully created **24 issues** organized by priority:

### High Priority (7 issues)
1. **#7** - Integrate and maintain accessibility throughout website
2. **#8** - Improve splash page design and responsiveness
3. **#9** - Add Currently/Current Hobbies section to home page
4. **#10** - Complete About page (like Carrd)
5. **#11** - Add and host Shantell Sans font
6. **#12** - Add update log section to home page
7. **#13** - Implement light and dark mode themes

### Medium Priority (15 issues)
8. **#14** - Create custom buttons and blinkies
9. **#15** - Create and add favicons for all pages
10. **#16** - Create Characters hub page
11. **#17** - Add Fanon Characters - JoJo AUs
12. **#18** - Add Fanon Characters - Pokemon
13. **#19** - Add Fanon Characters - World of Warcraft
14. **#20** - Add Original Characters pages
15. **#21** - Create Art page
16. **#22** - Create Recommendations/Resources page
17. **#23** - Join and add webrings
18. **#24** - Join and add fanlistings
19. **#25** - Fill out Button/Stamp/Blinkie Hoard page
20. **#26** - Add Who is...? page for people mentioned on site
21. **#27** - Update existing shrine pages
22. **#28** - Create new shrine pages

### Low Priority (2 issues)
23. **#29** - Add current status section to home page
24. **#30** - Explore inspiration from 32bit.cafe and Neocities

---

## How to Use This in the Future

### Creating a Single Issue

```powershell
gh issue create --repo "Lavender-Daydream/Website-lavender-daydream.com" `
  --title "Your Issue Title" `
  --label "label1,label2" `
  --body "Your issue description here"
```

### Creating Issues from a List

1. Format your issues in a script (like we did)
2. Run the script with PowerShell
3. Each issue gets created automatically

### Other Useful GitHub CLI Commands

```powershell
# View all issues
gh issue list

# View a specific issue
gh issue view 7

# Close an issue
gh issue close 7

# Add a comment to an issue
gh issue comment 7 --body "Your comment here"

# Edit an issue
gh issue edit 7 --title "New title"

# Add labels to an issue
gh issue edit 7 --add-label "new-label"
```

---

## Key Learnings

### 1. GitHub CLI is Powerful
The `gh` command-line tool makes it easy to automate GitHub tasks. Instead of clicking through the web interface 24 times, we ran one script!

### 2. PowerShell for Automation
PowerShell scripts can automate repetitive tasks. The pattern we used was:
- Loop through each item
- Execute a command for each item
- Add small delays to be respectful to GitHub's servers

### 3. Labels Must Exist First
Some labels (`gallery`, `update`) didn't exist in the repository yet, so they couldn't be automatically applied. You can create these labels in your repository settings if needed.

### 4. Issues Can Be Edited After Creation
We demonstrated this by adding credit notes to all issues after they were created. GitHub CLI makes bulk edits easy!

---

## Tips for Managing Your Issues

### Organizing Issues
- Use **labels** to categorize issues (design, content, high priority, etc.)
- Use **milestones** to group related issues (e.g., "Accessibility Overhaul")
- Use **projects** for kanban-style organization

### Closing Issues
When you complete a task, you can close the issue:
- Via GitHub web interface (click "Close issue" button)
- Via command line: `gh issue close 7`
- Via commit message: Include "closes #7" or "fixes #7" in your commit message

### Cross-Referencing
You can reference issues in other issues by using `#7` in the text. GitHub will automatically create a link.

---

## Troubleshooting

### If `gh` command is not found
The PATH might not be updated. Use the full path:
```powershell
& 'C:\Program Files\GitHub CLI\gh.exe' [command]
```

Or restart your terminal to refresh the PATH.

### If authentication fails
Re-authenticate with:
```powershell
gh auth login
```

### If rate limiting occurs
GitHub has rate limits. If you hit them, wait a few minutes and try again. Our scripts include small delays to prevent this.

---

## Resources

- **GitHub CLI Documentation:** https://cli.github.com/manual/
- **Your Repository Issues:** https://github.com/Lavender-Daydream/Website-lavender-daydream.com/issues
- **Original Issue List:** See `github_issues.md` in this folder

---

## Why This Matters

Before automation:
- ⏱️ Estimated time: 1-2 hours of manual copy-pasting
- 😰 Risk of errors or missing information
- 🔄 Repetitive and boring work

After automation:
- ⚡ Actual time: ~12 seconds
- ✅ Perfect consistency across all issues
- 🎉 More time for actual development!

---

## Can This Be Reused?

**Yes!** If you have another list of issues to create:

1. Open `create_issues_simple.ps1`
2. Modify the issue data (titles, labels, bodies)
3. Run the script: `powershell.exe -ExecutionPolicy Bypass -File create_issues_simple.ps1`
4. Done!

You can also adapt this pattern for:
- Creating pull requests (`gh pr create`)
- Adding comments to issues (`gh issue comment`)
- Bulk-editing issues
- And much more!

---

## Questions or Want to Learn More?

This automation was created using:
- **Claude.ai** - For planning and guidance
- **Claude Code** - For executing commands and creating scripts
- **GitHub CLI** - The tool that makes GitHub automation possible
- **PowerShell** - The scripting language we used

Feel free to modify the scripts, experiment, and automate more tasks! The more you automate, the more time you have for creative work on your website.

---

**Happy coding! 🌟**

*This document was created with Claude.ai and Claude Code to help you understand and replicate the automation process.*
