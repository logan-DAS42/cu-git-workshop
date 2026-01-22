# CLAUDE.md - AI Assistant Guide for cu-git-workshop

## Repository Overview

This is an educational Git workshop repository designed to teach GitHub collaboration workflows, primarily for students learning Git and GitHub basics. The repository serves as a hands-on learning environment where participants practice forking, branching, committing, and creating pull requests.

**Repository Purpose**: DAS42 GitHub Workshop training material and collaboration practice
**Primary Audience**: Students and workshop participants learning Git/GitHub
**Repository Owner**: logan-DAS42

## Repository Structure

```
cu-git-workshop/
├── README.md              # Workshop instructions and Git command reference
├── sign-in-sheet.txt      # Participant sign-in file (main collaboration point)
├── motivation.sh          # Simple shell script (prints "Git with it!")
└── CLAUDE.md             # This file - AI assistant guidance
```

### Key Files

1. **README.md** (1,860 bytes)
   - Contains setup instructions for workshop participants
   - Lists essential Git CLI commands with explanations
   - Provides guidance for GitHub account setup and Repl.it configuration
   - Reference for workshop participants

2. **sign-in-sheet.txt** (154 bytes)
   - Primary file for participant contributions
   - Simple format: `Full Name - Email`
   - Workshop participants add their information here
   - Common target for practice pull requests

3. **motivation.sh** (18 bytes)
   - Simple bash script that echoes "Git with it!"
   - Demonstrates basic shell scripting
   - Fun motivational element for workshop

## Development Workflows

### Standard Workshop Participant Flow

This repository uses a fork-and-pull-request workflow typical for open source contributions:

1. **Fork the repository** - Participants fork `logan-DAS42/cu-git-workshop` to their own GitHub account
2. **Clone locally** - Clone the forked repository to local machine or Repl.it
3. **Configure Git** - Set user.email and user.name
4. **Make changes** - Typically adding name/email to sign-in-sheet.txt
5. **Commit changes** - Create meaningful commit messages
6. **Push to fork** - Push changes to their forked repository
7. **Create Pull Request** - Submit PR from fork to original repository
8. **Review and Merge** - Workshop maintainer reviews and merges

### Branch Strategy

**Main Branch**: `master` (note: not `main`)
- This repository uses `master` as the default branch
- All PRs should target `master`
- Clean working state in recent commits

**Feature Branches**:
- Workshop participants may create feature branches
- Naming convention observed: descriptive names like `shubhika`, participant names
- AI assistants should follow the branch naming requirements specified in the session context

### Commit Patterns Observed

Analyzing recent commits shows these patterns:
- Simple, descriptive messages: "Updated sign-in sheet", "add name and email"
- Merge commit pattern: "Merge pull request #X from user/branch"
- Focus on incremental changes
- Educational context allows for learning-oriented commit messages

## AI Assistant Guidelines

### When Working in This Repository

1. **Respect the Educational Context**
   - This is a learning environment - clarity and simplicity are paramount
   - Avoid over-engineering solutions
   - Make changes that demonstrate good practices without being overly complex
   - Comments and explanations should be educational

2. **File Modification Priorities**
   - **sign-in-sheet.txt**: Most common modification - maintain format consistency
   - **README.md**: Only modify if improving workshop instructions or fixing errors
   - **motivation.sh**: Generally should not need modification
   - **New files**: Only create if explicitly requested or necessary for workshop enhancement

3. **Commit Message Guidelines**
   - Keep messages simple and descriptive
   - Use present tense: "Add", "Update", "Fix", not "Added", "Updated", "Fixed"
   - Examples from history:
     - ✓ "Updated sign-in sheet"
     - ✓ "add name and email"
     - ✓ "Update README.md"
   - For educational context, clarity trumps brevity

4. **Pull Request Best Practices**
   - Target branch: `master` (not `main`)
   - Title should be clear and descriptive
   - Body should explain what changed and why (educational value)
   - Reference any related issues or workshop tasks

### Git Configuration Expectations

Workshop participants are instructed to configure:
```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

AI assistants should:
- Not modify global git config
- Respect existing config settings
- Use provided branch naming conventions from session context

### Code Quality and Style

Since this is a minimal educational repository:
- **Shell scripts**: Simple, readable bash with clear output
- **Documentation**: Clear, beginner-friendly markdown
- **Text files**: Plain text, consistent formatting
- **No complex dependencies**: Keep it simple for workshop environment

### Testing and Validation

For this repository:
- No automated test suite exists
- Manual validation appropriate: check file syntax, verify changes
- For sign-in-sheet.txt: ensure proper formatting maintained
- For scripts: test execution, verify output

## Common Tasks for AI Assistants

### Task: Update Sign-In Sheet

**Process**:
1. Read current sign-in-sheet.txt
2. Append new entry maintaining format: `Full Name - Email`
3. Preserve existing formatting and line structure
4. Commit with message: "Add [name] to sign-in sheet"

**Example**:
```
Full Name - Email
-------------------------
Logan Guerry - logan@das42.com
Fairy Gandhi - Fairy.Gandhi@colordado.edu
Jaden Tuma - jaden.tuma@colorado.edu
[New Name] - [new.email@example.com]
```

### Task: Update Documentation

**Process**:
1. Read README.md thoroughly first
2. Identify section requiring update
3. Make minimal, targeted changes
4. Preserve existing structure and style
5. Commit with clear message describing what improved

### Task: Add New Workshop Content

**Process**:
1. Discuss with user to understand educational goal
2. Create simple, clear examples appropriate for beginners
3. Document any new files in this CLAUDE.md
4. Test any scripts or code before committing
5. Provide educational context in commit message

## Repository Conventions

### File Naming
- Use lowercase with hyphens: `sign-in-sheet.txt`
- Keep names descriptive and clear
- Avoid special characters except hyphens and underscores

### Line Endings
- Unix-style line endings (LF) preferred
- Consistent with Git best practices

### File Encoding
- UTF-8 encoding for all text files
- No BOM (Byte Order Mark)

## Workshop Context

### Target Audience
- University students (Colorado University, based on emails)
- Beginners to Git/GitHub
- May be using browser-based IDEs (Repl.it mentioned)

### Learning Objectives
Based on README.md, participants learn:
- Git CLI commands: clone, branch, checkout, status, fetch, pull, add, rm, commit, push
- GitHub account setup and navigation
- Fork and pull request workflow
- Basic repository collaboration

### Common Participant Challenges
AI assistants should be prepared to help with:
- First-time Git setup (config user.name, user.email)
- Understanding the difference between local and remote
- Commit message best practices
- Pull request creation process
- Merge conflict resolution (if it occurs)

## Integration Points

### External Services Mentioned
- **GitHub**: Primary hosting platform
- **Repl.it**: Recommended IDE for workshop participants
  - Browser-based, no local setup required
  - Supports Git operations
  - Google SSO authentication suggested with CU email

### Remote Repository
- Owner: logan-DAS42
- Repository: cu-git-workshop
- Default branch: master
- Fork-friendly: designed for multiple forks and contributions

## Change History and Evolution

### Repository History Insights
- Multiple merged pull requests from workshop participants
- Contributors include: FairyGandhi, bigTuma, shubhika27, AlanMarket
- Active educational use with regular participant contributions
- Merge pattern shows successful completion of workshop exercises

### Maintenance Expectations
- Workshop instructor (logan-DAS42) reviews and merges PRs
- Simple, permissive acceptance criteria for learning purposes
- Focus on process over perfection

## AI Assistant Best Practices Summary

### DO:
✓ Keep changes simple and educational
✓ Maintain consistent formatting in sign-in-sheet.txt
✓ Write clear, beginner-friendly commit messages
✓ Target `master` branch for pull requests
✓ Respect the learning environment context
✓ Test any scripts before committing
✓ Provide explanations that enhance learning
✓ Follow session-specific branch naming requirements

### DON'T:
✗ Over-engineer solutions
✗ Add complex dependencies or tooling
✗ Modify git config without explicit instruction
✗ Create unnecessary files
✗ Use overly technical commit messages
✗ Push directly to master (use PRs as instructed in session context)
✗ Skip reading existing files before modifications
✗ Assume `main` branch (it's `master` here)

## Quick Reference Commands

```bash
# Initial setup (for participants)
git clone <REPO_URL>
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

# Standard workflow
git status                    # Check current state
git add <file>               # Stage changes
git commit -m "message"      # Commit changes
git push -u origin <branch>  # Push to remote

# Branch operations
git branch                   # List branches
git checkout -b <branch>     # Create and switch to new branch
git checkout <branch>        # Switch branches

# Syncing with upstream
git fetch origin            # Fetch changes
git pull origin master      # Pull and merge changes
```

## Version Information

- **Created**: 2026-01-22
- **Last Updated**: 2026-01-22
- **Repository State**: Clean working directory on branch `claude/add-claude-documentation-kLk7s`
- **Recent HEAD**: c0b2810 "Merge pull request #10 from FairyGandhi/master"

## Additional Notes

This CLAUDE.md file should be updated when:
- New workshop materials are added
- Repository structure changes
- New conventions are established
- Workshop format or objectives evolve
- Integration with new tools or platforms

For questions about this repository or suggested improvements to this guide, contact the repository owner or submit a pull request with proposed changes.

---

*This file serves as a comprehensive guide for AI assistants working in the cu-git-workshop repository. It is designed to ensure AI assistants understand the educational context, maintain consistency with established practices, and provide maximum value to workshop participants and instructors.*
