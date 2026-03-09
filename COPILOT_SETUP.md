# GitHub Copilot Setup Guide for Movie App

This guide will help you set up and troubleshoot GitHub Copilot in VS Code for this project.

## Prerequisites

1. **GitHub Copilot Subscription**: You need an active GitHub Copilot subscription. Students can get it for free through the [GitHub Student Developer Pack](https://education.github.com/pack).

2. **Visual Studio Code**: Download and install [VS Code](https://code.visualstudio.com/) if you haven't already.

## Installation Steps

### Step 1: Install Required Extensions

1. Open VS Code
2. Go to the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
3. Search for and install the following extensions:
   - **GitHub Copilot** (`github.copilot`)
   - **GitHub Copilot Chat** (`github.copilot-chat`)

Alternatively, when you open this project in VS Code, it will automatically recommend these extensions. Just click "Install All" when prompted.

### Step 2: Sign in to GitHub

1. After installing the extensions, you'll be prompted to sign in to GitHub
2. Click on the **Sign in to GitHub** button
3. A browser window will open - authorize VS Code to access your GitHub account
4. Return to VS Code after authorization

### Step 3: Verify GitHub Copilot is Active

1. Look for the Copilot icon in the VS Code status bar (bottom right)
2. The icon should show as active (not crossed out)
3. Click on it to see your Copilot status

## Using GitHub Copilot Features

> 💡 **Not sure if Copilot Pro is working?** See the [Copilot Pro Verification Guide](VERIFY_COPILOT_PRO.md) to confirm your setup!

### Inline Code Suggestions

- Start typing code, and Copilot will suggest completions
- Press `Tab` to accept a suggestion
- Press `Esc` to dismiss a suggestion
- Press `Alt+]` or `Option+]` to see the next suggestion
- Press `Alt+[` or `Option+[` to see the previous suggestion

### GitHub Copilot Chat

1. Open Copilot Chat using:
   - Click the chat icon in the Activity Bar (left sidebar)
   - Use keyboard shortcut: `Ctrl+Shift+I` or `Cmd+Shift+I` on Mac
   - Or use Command Palette: `Ctrl+Shift+P` → "GitHub Copilot: Open Chat"

2. **Ask questions** about your code:
   - "How does this component work?"
   - "Explain this function"
   - "Help me optimize this code"

3. **Use Workspace Features**:
   - Use `@workspace` to ask questions about the entire codebase
   - Example: "@workspace how is movie data fetched?"
   - Example: "@workspace explain the routing structure"

### Model Selection in Copilot Chat

When GitHub Copilot Pro is properly activated, you can select different models:

1. Open Copilot Chat
2. Look for the model selector at the top of the chat panel
3. Available models may include:
   - GPT-4 (default for Pro users)
   - GPT-3.5-turbo
   - Claude (if available)

**Note**: Model selection is only available for GitHub Copilot Pro/Enterprise subscribers.

## Troubleshooting

### Issue 1: Can't see workspace features or model selection

**Symptoms**: 
- No model selector in Copilot Chat
- @workspace commands don't work
- Limited Copilot features

**Solutions**:

1. **Verify your subscription**:
   - Go to [GitHub Copilot Settings](https://github.com/settings/copilot)
   - Ensure your GitHub Copilot subscription is active
   - For students: Verify your [Student Developer Pack](https://education.github.com/pack) is approved

2. **Check extension versions**:
   - Ensure you have the latest versions of:
     - GitHub Copilot extension
     - GitHub Copilot Chat extension
   - Update extensions: Extensions view → Click the gear icon on each extension → "Update"

3. **Sign out and sign in again**:
   - Click the Copilot icon in the status bar
   - Select "Sign Out"
   - Sign in again with your GitHub account

4. **Verify authentication**:
   - Click on the Account icon (bottom left in VS Code)
   - Ensure you're signed in with the correct GitHub account that has Copilot access
   - If multiple accounts, make sure the one with Copilot is selected

5. **Reload VS Code**:
   - Open Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`)
   - Type "Developer: Reload Window"
   - Press Enter

### Issue 2: Copilot icon shows "Not Active" or has an X

**Solutions**:

1. Check your internet connection
2. Sign out and sign back in to GitHub in VS Code
3. Restart VS Code completely
4. Check [GitHub Status](https://www.githubstatus.com/) for any service outages

### Issue 3: Copilot Chat not opening

**Solutions**:

1. Ensure the GitHub Copilot Chat extension is installed
2. Try the keyboard shortcut: `Ctrl+Shift+I` (or `Cmd+Shift+I` on Mac)
3. Check if the chat icon appears in the Activity Bar (left sidebar)
4. If not visible, right-click on the Activity Bar and ensure "GitHub Copilot Chat" is checked

### Issue 4: No code suggestions appearing

**Solutions**:

1. Check that Copilot is enabled for the current file type:
   - Open settings (`Ctrl+,` or `Cmd+,`)
   - Search for "copilot enable"
   - Ensure JavaScript/React is enabled

2. Verify the file is not too large (Copilot may not work on very large files)

3. Check if you're in a supported file type (`.js`, `.jsx`, etc.)

### Issue 5: Student Developer Pack Benefits Not Working

**Solutions**:

1. **Verify student pack approval**:
   - Go to [GitHub Education](https://education.github.com/)
   - Check that your student status is verified and approved
   - This process can take a few days after application

2. **Enable Copilot after approval**:
   - Once approved, go to [GitHub Copilot Settings](https://github.com/settings/copilot)
   - Enable GitHub Copilot for your account

3. **Wait for propagation**:
   - After enabling, it may take a few minutes for the changes to propagate
   - Sign out and back in to VS Code
   - Restart VS Code

### Issue 6: "Language model unavailable" Error

**Symptoms**:
- Specific models (e.g., GPT-5.3, GPT-5.4) show "Language model unavailable" error
- Models worked yesterday but not today
- Error appears when trying to use certain models in Copilot Chat
- Other models may still work fine

**Important**: This is **NOT** a Copilot Pro subscription issue! If you can see the model selector with multiple models, your Pro subscription is working correctly. This is a temporary model availability issue.

**Common Causes**:

1. **Temporary Service Issues**
   - GitHub's AI model services experience temporary outages
   - Specific models may be under maintenance
   - High demand can cause temporary unavailability

2. **Rate Limiting**
   - You may have exceeded usage limits for a specific model
   - Different models have different rate limits
   - Limits typically reset after a few hours

3. **Model Deployment Updates**
   - GitHub periodically updates or rotates AI models
   - Some models may be temporarily offline during updates
   - New model versions may be rolling out

**Solutions**:

1. **Switch to a Different Model** (Immediate workaround)
   - Click the model selector at the top of Copilot Chat
   - Choose a different available model (e.g., if GPT-5.4 is unavailable, try GPT-5.3-Codex, Gemini, or another model)
   - All models are powerful - you'll get excellent results with any available model
   
   Example: If you see:
   ```
   ✅ GPT-5.3-Codex - Available
   ❌ GPT-5.4 - Language model unavailable
   ✅ Gemini 2.5 Pro - Available
   ```
   Just use GPT-5.3-Codex or Gemini instead!

2. **Wait and Retry**
   - Model availability issues are usually temporary (minutes to hours)
   - Try again in 15-30 minutes
   - Most issues resolve within a few hours
   - The model will automatically become available again once service is restored

3. **Check GitHub Status**
   - Visit [GitHub Status](https://www.githubstatus.com/)
   - Look for any reported issues with "Copilot" or "AI Services"
   - Check if there are ongoing incidents or maintenance

4. **Verify It's Not a Subscription Issue**
   - If ALL models show as unavailable → might be a subscription/auth issue (see Issue 1)
   - If ONLY specific models are unavailable → it's a temporary availability issue (normal!)
   - Being able to see the model dropdown = Your Pro subscription is fine ✅

5. **Clear and Reload**
   - Open Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`)
   - Type "Developer: Reload Window"
   - Try the model again after reload

6. **Update Extensions**
   - Sometimes model availability improves with extension updates
   - Go to Extensions view (`Ctrl+Shift+X`)
   - Check for updates to GitHub Copilot and GitHub Copilot Chat extensions
   - Update if available, then reload VS Code

**What You Should Know**:

✅ **This is NORMAL**: Model unavailability happens occasionally to all users  
✅ **You still have Pro**: Seeing the model selector = Pro is working  
✅ **Use other models**: All available models are excellent alternatives  
✅ **It's temporary**: Models usually return to availability within hours  
✅ **Not your fault**: This is a service-side issue, not something you caused  

**Best Practice**:
- Bookmark 2-3 favorite models that you like
- If your primary choice is unavailable, switch to your backup
- Don't wait - be productive with whichever models are available!

**Still Having Issues After 24 Hours?**
- Check [GitHub Community Discussions](https://github.com/orgs/community/discussions/categories/copilot)
- Contact [GitHub Support](https://support.github.com/)
- Verify your subscription is still active at [GitHub Copilot Settings](https://github.com/settings/copilot)

## Advanced Features for This Project

### Using Copilot with React

1. **Component generation**: Start typing a component name and let Copilot suggest the structure
2. **Hook suggestions**: Type "useState" or "useEffect" and get context-aware suggestions
3. **Event handlers**: Start typing "handle" and get relevant event handler suggestions

### Workspace Context

When using `@workspace` in Copilot Chat, you can ask:
- "@workspace how does the movie search work?"
- "@workspace explain the rating component"
- "@workspace what hooks are used in this project?"
- "@workspace how is local storage implemented?"

### Code Explanation

Select any code block and:
1. Right-click → "Copilot" → "Explain This"
2. Or use the chat: "Explain the selected code"

## Additional Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [GitHub Copilot in VS Code](https://code.visualstudio.com/docs/editor/github-copilot)
- [GitHub Student Developer Pack](https://education.github.com/pack)
- [GitHub Copilot Chat Documentation](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat-in-your-ide)

## Need More Help?

If you're still experiencing issues:

1. Check the [GitHub Copilot Community Discussions](https://github.com/orgs/community/discussions/categories/copilot)
2. Review the [VS Code Copilot Troubleshooting Guide](https://code.visualstudio.com/docs/editor/github-copilot#_troubleshooting)
3. Contact [GitHub Support](https://support.github.com/) if you have subscription issues
4. For student pack issues, contact [GitHub Education Support](https://support.github.com/contact/education)

## Project-Specific Setup

This project is a React movie application. Copilot works best when:
- You have the recommended extensions installed (see `.vscode/extensions.json`)
- You're working with JavaScript/React files (`.js`, `.jsx`)
- You provide clear context in comments when asking for help
- You use descriptive variable and function names

Happy coding with GitHub Copilot! 🚀
