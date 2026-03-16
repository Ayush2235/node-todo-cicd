# node-todo-cicd

A simple Node.js todo list application with CI/CD pipeline.

## Installation

Run these commands:

```bash
sudo apt install nodejs
sudo apt install npm
npm install
node app.js
```

Or run by docker compose:

```bash
docker-compose up
```

## VS Code Copilot Chat - Claude Models

If you're looking to use Claude models (like Claude Sonnet 4.5) in VS Code Copilot Chat, please see the detailed setup guide:

📖 **[VS Code Copilot Claude Setup Guide](./VSCODE_COPILOT_CLAUDE_SETUP.md)**

**Quick Summary**:
- Claude model availability in GitHub Copilot depends on your subscription tier and GitHub's rollout
- This repository includes `.vscode/settings.json` with Claude model preferences pre-configured
- If Claude models aren't available in your Copilot, consider using [Claude Code](https://github.com/anthropics/claude-code) or [Claude.ai](https://claude.ai) directly

## Testing

```bash
npm test
```
