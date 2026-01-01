# Claude Code on Windows (No Admin Rights)

This guide documents a **working setup** for installing and running **Claude Code** on a Windows machine **without administrator rights**, using **Git Bash** and a **manual `.bash_profile` approach**.

---

## 1. Install Git Bash (Git for Windows)

Download Git for Windows from the **official site**:

https://git-scm.com/download/win

This installs **Git Bash**, which provides `bash.exe`.  
Claude Code **requires** a Bash shell on Windows.

> ⚠️ PowerShell alone is not sufficient.

---

## 2. Install Node.js (No Admin, ZIP Method)

Download **Node.js LTS (Windows ZIP, x64)** from:

https://nodejs.org/en/download

Choose:
- Windows
- ZIP (.zip)
- LTS
- x64

Do **not** use the MSI installer.

Extract the ZIP manually to:

```
C:\Users\<you>\node\node-v20.x.x-win-x64
```

You should see `node.exe` inside that folder.

---

## 3. Manually Configure Environment (`.bash_profile`)

Git Bash on Windows does **not reliably create or source `.bashrc`**, so we use a **manual `.bash_profile`** approach.

Create or edit the file:

```bash
nano ~/.bash_profile
```

Add the following lines (adjust paths if needed):

```bash
export PATH="$HOME/node/node-v20.11.1-win-x64:$PATH"
export CLAUDE_CODE_GIT_BASH_PATH="/c/Users/<you>/AppData/Local/Programs/Git/bin/bash.exe"
```

Save and reload:

```bash
source ~/.bash_profile
```

Verify Node is available:

```bash
node -v
npm -v
```

---

## 4. Install Claude Code

With Node available:

```bash
npm install -g @anthropic-ai/claude-code
```

Verify installation:

```bash
claude --version
```

---

## 5. Authenticate Claude Code

```bash
claude auth login
```

This opens a browser to authenticate your Claude / Anthropic account.

---

## 6. Use Claude Code

Navigate to a project directory and launch Claude:

```bash
cd <your-project>
claude
```

Claude will now operate **repo-aware** inside that directory.

---

## Windows-Specific Gotchas (Important)

- Claude Code **requires Git Bash**, not PowerShell
- `bash.exe` must be discoverable:
  - Set `CLAUDE_CODE_GIT_BASH_PATH` explicitly
- Use **Windows Node ZIP**, not Linux/macOS builds
- `.bash_profile` works more reliably than `.bashrc` on Git Bash
- Use Unix-style paths (`/c/...`) inside Git Bash

---

## Quick Sanity Check

All of the following should work:

```bash
node -v
npm -v
echo $CLAUDE_CODE_GIT_BASH_PATH
ls "$CLAUDE_CODE_GIT_BASH_PATH"
claude
```

---

## Status

✅ Confirmed working  
✅ No admin rights required  
✅ Suitable for locked-down corporate laptops  

