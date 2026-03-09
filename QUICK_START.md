# Quick Start Cheat Sheet - GitHub Copilot Pro

Use this as a quick reference after completing the [Getting Started Guide](GETTING_STARTED_COPILOT_PRO.md).

## 🏃 Quick Setup (5 Minutes)

If you already have VS Code and Git installed:

```bash
# 1. Clone the repo
git clone https://github.com/mehari06/movie-app.git
cd movie-app

# 2. Install dependencies
npm install

# 3. Open in VS Code
code .

# 4. Install Copilot extensions (when prompted, click "Install All")
# 5. Sign in to GitHub (click account icon, bottom left)
# 6. Start coding! (open App.js and start typing)

# 7. Run the app
npm start
```

## ⌨️ Essential Keyboard Shortcuts

| What | Windows/Linux | Mac |
|------|---------------|-----|
| **Open Copilot Chat** | `Ctrl+Shift+I` | `Cmd+Shift+I` |
| **Accept suggestion** | `Tab` | `Tab` |
| **Next suggestion** | `Alt+]` | `Option+]` |
| **Command Palette** | `Ctrl+Shift+P` | `Cmd+Shift+P` |
| **Terminal** | `` Ctrl+` `` | `` Cmd+` `` |

## 💬 Copilot Chat Commands

```
@workspace What does this app do?
@workspace How does movie search work?
@workspace Explain the StarRating component

/explain [select code first]
/fix [select code with issues]
/tests [select function]
```

## 🎯 First Things to Try

1. **Open `App.js`** and add a comment:
   ```javascript
   // Function to sort movies by rating
   ```
   Press Enter → Tab to accept Copilot's suggestion

2. **Ask in Chat**:
   ```
   @workspace Give me a tour of this codebase
   ```

3. **Select some code**, right-click → Copilot → Explain This

4. **Run the app**:
   ```bash
   npm start
   ```

## ✅ Is Everything Working?

- [ ] Copilot icon `><` in bottom right (not crossed out)
- [ ] Chat opens with `Ctrl+Shift+I` / `Cmd+Shift+I`
- [ ] Model selector visible at top of chat (GPT-4, etc.)
- [ ] `@workspace` commands work in chat
- [ ] Typing shows gray suggestions you can Tab to accept
- [ ] `npm start` runs the app at http://localhost:3000

## 🔧 Quick Fixes

**Copilot not working?**
→ Click the `><` icon → Sign in

**No suggestions?**
→ Make sure you're editing a `.js` file
→ Try typing a comment then press Enter

**No @workspace?**
→ You might have regular Copilot, not Pro
→ Check: https://github.com/settings/copilot

**npm install fails?**
→ Install Node.js from https://nodejs.org/
→ Run `node --version` to verify

## 📚 Full Guides

- **Complete setup**: [GETTING_STARTED_COPILOT_PRO.md](GETTING_STARTED_COPILOT_PRO.md)
- **Troubleshooting**: [COPILOT_SETUP.md](COPILOT_SETUP.md)
- **Project info**: [README.md](README.md)

## 🎓 Learning Path

**Day 1**: Get familiar with inline suggestions
- Open files, type comments, accept suggestions with Tab

**Day 2**: Learn chat features
- Ask questions about the code with `@workspace`
- Use `/explain` and `/fix` commands

**Day 3**: Switch models and compare
- Try GPT-4 for complex questions
- Try GPT-3.5 for quick answers

**Week 2+**: Build something new
- Ask Copilot to help add features
- "How can I add a favorites list?"
- "How can I add movie trailers?"

---

**Need detailed help?** → [GETTING_STARTED_COPILOT_PRO.md](GETTING_STARTED_COPILOT_PRO.md)

**Questions?** → Ask in Copilot Chat: "I need help with [your issue]"
