# VS Code Copilot Chat - Claude Models Setup Guide

## Issue
Cannot see Claude Sonnet 4.5 or other Claude models in VS Code Copilot Chat.

## Solution

### Prerequisites
1. **GitHub Copilot Subscription**: You need an active GitHub Copilot subscription
   - Individual: https://github.com/settings/copilot
   - Business/Enterprise: Contact your organization admin

2. **VS Code Extensions**: Install the required extensions
   - GitHub Copilot (`GitHub.copilot`)
   - GitHub Copilot Chat (`GitHub.copilot-chat`)

### Steps to Enable Claude Models in VS Code Copilot

#### Method 1: Using VS Code Settings UI
1. Open VS Code Settings (`Ctrl+,` or `Cmd+,`)
2. Search for "Copilot Chat Model"
3. Select your preferred Claude model from the dropdown:
   - `claude-3.5-sonnet` (Claude Sonnet 3.5)
   - `claude-sonnet-4.5` (Claude Sonnet 4.5) - if available
   - `claude-opus` (Claude Opus) - if available

#### Method 2: Using settings.json (Already Configured)
This repository includes `.vscode/settings.json` with pre-configured settings for Claude models.

The settings include:
```json
{
  "github.copilot.chat.model": "claude-3.5-sonnet"
}
```

#### Method 3: In-Chat Model Selection
1. Open GitHub Copilot Chat panel (`Ctrl+Shift+I` or `Cmd+Shift+I`)
2. Click on the model selector dropdown at the top of the chat
3. Select your preferred Claude model

### Important Notes

#### Model Availability
- **Claude model availability depends on your GitHub Copilot plan and region**
- GitHub Copilot Individual (as of 2025): Primarily uses GPT-4 and GPT-3.5 models
- GitHub Copilot Business/Enterprise: May have access to Claude models depending on organization settings
- **Claude models in Copilot are rolling out gradually** and may not be available to all users yet

#### Current Status (March 2026)
GitHub Copilot's model offerings are continuously evolving. As of the knowledge cutoff:
- GPT-4 and GPT-3.5-Turbo are the primary models
- Claude model integration is being tested/rolled out
- Model availability varies by subscription tier

### Troubleshooting

#### If Claude models are not showing:

1. **Check Copilot Subscription Status**
   ```
   - Go to https://github.com/settings/copilot
   - Verify your subscription is active
   - Check your subscription tier
   ```

2. **Verify Extension Versions**
   - Update GitHub Copilot extensions to the latest version
   - Restart VS Code after updating

3. **Check Organization Policies** (for Business/Enterprise users)
   - Contact your GitHub organization admin
   - Verify that Claude models are enabled in organization settings

4. **Region/Account Limitations**
   - Some models may be region-specific
   - Beta features might require opt-in

5. **Alternative: Use Claude Directly**
   If Claude models are not available in Copilot, consider:
   - **Claude Code CLI**: https://github.com/anthropics/claude-code
   - **Claude.ai Web Interface**: https://claude.ai
   - **Anthropic API**: Direct API integration
   - **Continue.dev**: VS Code extension with Claude support

### Using Claude Code Extension Instead

If you want guaranteed access to Claude Sonnet 4.5 and other Claude models in VS Code, consider using the official Claude Code extension:

1. Install Claude Code: https://github.com/anthropics/claude-code
2. Get an Anthropic API key: https://console.anthropic.com/
3. Configure in VS Code settings

## References
- GitHub Copilot Documentation: https://docs.github.com/en/copilot
- GitHub Copilot Models: https://docs.github.com/en/copilot/using-github-copilot/asking-github-copilot-questions-in-your-ide
- Claude Documentation: https://docs.anthropic.com/
- Claude Code: https://github.com/anthropics/claude-code

## For This Repository

The `.vscode/settings.json` file in this repository attempts to configure Claude as the preferred model. However, actual model availability depends on your GitHub Copilot subscription and GitHub's rollout schedule.

If Claude models are not available in your Copilot Chat, this is a **GitHub/Copilot limitation**, not an issue with this repository or its configuration.
