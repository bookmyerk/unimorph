# Opening UniMorph in VS Code

This repository now includes VS Code workspace configuration files to make development easier.

## Quick Start

### Option 1: Open the Workspace File (Recommended)
1. Open VS Code
2. Click **File > Open Workspace from File...**
3. Navigate to and select `unimorph.code-workspace`
4. VS Code will open the workspace with all configured settings

### Option 2: Open the Folder
1. Open VS Code
2. Click **File > Open Folder...**
3. Navigate to and select the `unimorph` directory
4. VS Code will automatically detect the `.vscode` settings

## What's Included

### Settings (`.vscode/settings.json`)
- UTF-8 encoding for all files
- Unix-style line endings (LF)
- Automatic trailing whitespace removal
- Tab size of 2 spaces
- Proper file associations for shell scripts and markdown
- Git submodule support

### Recommended Extensions (`.vscode/extensions.json`)
When you open the workspace, VS Code will suggest installing these helpful extensions:
- **ShellCheck** - Linting for shell scripts (like `download_all.sh`)
- **Shell Format** - Formatting for shell scripts
- **Markdown All in One** - Enhanced markdown editing features
- **Markdown Lint** - Linting for markdown files
- **Git Graph** - Visual git history (helpful for managing submodules)

## Working with Submodules

This repository uses git submodules to manage language data. The workspace configuration includes:
- Submodule tracking enabled
- Git Graph extension recommended for visualizing submodule states

To update all submodules:
```bash
git submodule update --init --recursive
```

## Need Help?

See the main [README.md](README.md) and [versioning_guideline.md](versioning_guideline.md) for more information about the UniMorph project.
