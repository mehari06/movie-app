# Getting Started with GitHub Copilot Pro - Step by Step Guide

This is a complete step-by-step guide to get GitHub Copilot Pro working in VS Code with this movie app project. Follow these steps in order, and you'll be up and running in no time!

> **Already set up and just need a quick reference?** Check out the [Quick Start Cheat Sheet](QUICK_START.md)!

## 📋 What You'll Need

Before we start, make sure you have:
- A GitHub account
- GitHub Copilot Pro subscription (or Student Developer Pack access)
- Internet connection
- A computer (Windows, Mac, or Linux)

---

## Step 1: Get GitHub Copilot Pro Access

### Option A: If You're a Student (FREE!)

1. **Apply for GitHub Student Developer Pack**:
   - Go to: https://education.github.com/pack
   - Click "Get your pack"
   - Verify your student status (you'll need a .edu email or student ID)
   - Wait for approval (can take a few hours to a few days)

2. **Check your approval status**:
   - Go to: https://education.github.com/
   - Look for a green checkmark or "Verified" status
   - Once approved, proceed to Step 2

### Option B: If You're Not a Student

1. **Subscribe to GitHub Copilot**:
   - Go to: https://github.com/settings/copilot
   - Click "Enable GitHub Copilot"
   - Choose your subscription plan
   - Complete the payment process

2. **Verify your subscription**:
   - Go to: https://github.com/settings/copilot
   - You should see "GitHub Copilot is active"

✅ **Checkpoint**: Visit https://github.com/settings/copilot - you should see that Copilot is enabled for your account.

---

## Step 2: Install Visual Studio Code

1. **Download VS Code**:
   - Go to: https://code.visualstudio.com/
   - Click "Download for [Your Operating System]"
   - Download will start automatically

2. **Install VS Code**:
   - **Windows**: Run the downloaded `.exe` file, follow the installer
   - **Mac**: Open the downloaded `.dmg` file, drag VS Code to Applications
   - **Linux**: Follow instructions for your distribution

3. **Launch VS Code**:
   - Open VS Code from your applications menu
   - You should see the Welcome screen

✅ **Checkpoint**: VS Code is open and running on your computer.

---

## Step 3: Install Git (if you don't have it)

1. **Check if Git is installed**:
   - Open VS Code
   - Press `` Ctrl+` `` (or `Cmd+` on Mac) to open the terminal
   - Type: `git --version`
   - If you see a version number, Git is installed - **skip to Step 4**

2. **Install Git if needed**:
   - **Windows**: Download from https://git-scm.com/download/win
   - **Mac**: Open Terminal and type `git` - macOS will prompt to install
   - **Linux**: `sudo apt-get install git` (Ubuntu/Debian) or `sudo yum install git` (Fedora)

3. **Verify installation**:
   - Close and reopen VS Code terminal
   - Type: `git --version`
   - You should see the Git version

✅ **Checkpoint**: Running `git --version` shows a version number.

---

## Step 4: Clone This Repository

Now let's get the movie app code on your computer!

1. **Copy the repository URL**:
   - The URL is: `https://github.com/mehari06/movie-app.git`

2. **Open VS Code terminal**:
   - Press `` Ctrl+` `` (or `Cmd+` on Mac)

3. **Navigate to where you want the project**:
   ```bash
   # Example: Go to your Documents folder
   cd Documents
   
   # Or create a projects folder
   mkdir projects
   cd projects
   ```

4. **Clone the repository**:
   ```bash
   git clone https://github.com/mehari06/movie-app.git
   ```
   
   You should see:
   ```
   Cloning into 'movie-app'...
   remote: Enumerating objects...
   Unpacking objects: 100%...
   ```

5. **Open the project in VS Code**:
   ```bash
   cd movie-app
   code .
   ```
   
   Or use: File → Open Folder → Select the `movie-app` folder

✅ **Checkpoint**: VS Code shows the movie-app folder with files like `App.js`, `package.json`, etc. in the Explorer panel (left side).

---

## Step 5: Install Node.js and Dependencies

The movie app is a React project and needs Node.js to run.

1. **Check if Node.js is installed**:
   - In VS Code terminal, type: `node --version`
   - If you see a version number (v14 or higher), **skip to step 3**

2. **Install Node.js if needed**:
   - Go to: https://nodejs.org/
   - Download the LTS (Long Term Support) version
   - Install it (use default settings)
   - Restart VS Code

3. **Install project dependencies**:
   - In VS Code terminal, make sure you're in the movie-app folder
   - Run:
   ```bash
   npm install
   ```
   
   This will take a minute or two. You'll see a progress bar.

4. **Verify installation**:
   - You should see a `node_modules` folder appear in your project
   - The terminal should show "added XXX packages"

✅ **Checkpoint**: `npm install` completed successfully, and you have a `node_modules` folder.

---

## Step 6: Install GitHub Copilot Extensions

Now for the exciting part - adding Copilot to VS Code!

1. **You'll see a popup recommendation**:
   - When you opened the project, VS Code should show:
     "This workspace has extension recommendations"
   - Click **"Install All"**
   - This will install GitHub Copilot, Copilot Chat, and other helpful extensions

2. **Or install manually**:
   - Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on Mac) to open Extensions
   - Search for: `GitHub Copilot`
   - Click **Install** on "GitHub Copilot" by GitHub
   - Search for: `GitHub Copilot Chat`
   - Click **Install** on "GitHub Copilot Chat" by GitHub

3. **Wait for installation**:
   - The extensions will download and install
   - You might see a "Reload Required" button - click it

✅ **Checkpoint**: In the Extensions panel, both "GitHub Copilot" and "GitHub Copilot Chat" show "Installed" (not "Install").

---

## Step 7: Sign In to GitHub in VS Code

Connect VS Code to your GitHub account:

1. **Look for the sign-in prompt**:
   - After installing Copilot, you'll see a notification
   - Click **"Sign in to use GitHub Copilot"**

2. **Or sign in manually**:
   - Click the account icon (bottom left corner of VS Code)
   - Click **"Sign in to sync settings"** or **"Sign in to use GitHub Copilot"**
   - Choose **"Sign in with GitHub"**

3. **Authorize in browser**:
   - Your browser will open
   - Click **"Authorize Visual-Studio-Code"**
   - Enter your GitHub password if prompted
   - You'll see "Success! You may close this page"

4. **Return to VS Code**:
   - Go back to VS Code
   - You should see your GitHub username in the bottom left

✅ **Checkpoint**: Bottom left corner shows your GitHub username/profile picture.

---

## Step 8: Verify GitHub Copilot Pro is Active

Let's make sure everything is connected:

1. **Check the Copilot icon**:
   - Look at the bottom right of VS Code (status bar)
   - You should see a Copilot icon that looks like: `><`
   - The icon should **NOT** have an X through it

2. **Click the Copilot icon**:
   - Click on the `><` icon
   - You should see "GitHub Copilot is enabled"
   - It might also show "GPT-4" if you have Pro

3. **Check your subscription status**:
   - Open Copilot Chat (more on this in Step 9)
   - Type: "What subscription do I have?"
   - Copilot should confirm you have Pro access

4. **If something's wrong**:
   - Icon has an X: Click it and follow the "Sign in" prompts
   - Says "Not authorized": Go to https://github.com/settings/copilot and enable it
   - Still issues: See [COPILOT_SETUP.md](COPILOT_SETUP.md) for detailed troubleshooting

✅ **Checkpoint**: Copilot icon in status bar is active (no X), and clicking it shows "enabled".

---

## Step 9: Open and Use GitHub Copilot Chat

Time to interact with your AI coding assistant!

1. **Open Copilot Chat**:
   - Click the chat icon in the left sidebar (Activity Bar)
   - Or press: `Ctrl+Shift+I` (Windows/Linux) or `Cmd+Shift+I` (Mac)
   - Or: Press `Ctrl+Shift+P`, type "Copilot Chat", select "GitHub Copilot: Open Chat"

2. **Chat panel opens**:
   - You'll see a chat interface on the side
   - At the top, you might see a model selector (GPT-4, etc.)
   - At the bottom is a text input box
   - **See multiple models?** 🎉 [Verify your Pro is working!](VERIFY_COPILOT_PRO.md)

3. **Try your first question**:
   Type in the chat:
   ```
   @workspace What does this movie app do?
   ```
   
   Copilot will analyze the project and explain it!

4. **Try the workspace features** (Pro feature!):
   - `@workspace` - Ask about the entire project
   - `@workspace how does movie search work?`
   - `@workspace explain the StarRating component`
   - `@workspace what APIs does this use?`

✅ **Checkpoint**: Copilot Chat is open, and `@workspace` commands work and give you answers about the project.

---

## Step 10: Test Inline Code Suggestions

Let's see Copilot helping you code in real-time!

1. **Open a JavaScript file**:
   - In the Explorer (left sidebar), click on `App.js`

2. **Go to the bottom of the file**:
   - Scroll to the end
   - Add a few blank lines

3. **Start typing a comment**:
   ```javascript
   // Function to calculate average rating
   ```

4. **Press Enter and watch the magic**:
   - Copilot will suggest code in gray text
   - Press `Tab` to accept the suggestion
   - Press `Esc` to reject it
   - Press `Alt+]` to see alternative suggestions

5. **Try more examples**:
   ```javascript
   // Function to format movie duration from minutes to hours and minutes
   ```
   
   Copilot will suggest the implementation!

✅ **Checkpoint**: Typing comments or function names shows gray suggestion text that you can accept with Tab.

---

## Step 11: Test the Movie App Itself

Let's run the actual React app!

1. **Start the development server**:
   - In VS Code terminal, type:
   ```bash
   npm start
   ```

2. **Wait for it to compile**:
   - You'll see "Compiling..."
   - Then: "Compiled successfully!"
   - Your browser should automatically open to http://localhost:3000

3. **See the app running**:
   - You should see the movie app interface
   - Try searching for a movie (e.g., "Inception")
   - Click on a movie to see details

4. **Make a change with Copilot's help**:
   - Go back to VS Code
   - Open `App.js`
   - In the chat, ask: "How can I change the background color of the app?"
   - Follow Copilot's suggestions

5. **See your changes**:
   - The browser will auto-reload
   - You'll see your changes immediately!

✅ **Checkpoint**: Movie app is running in your browser, and you can search for movies.

---

## Step 12: Practice Using Copilot Pro Features

Now that everything works, let's explore what you can do!

### Model Selection (Pro Feature)

1. **Select a different AI model**:
   - Open Copilot Chat
   - Look at the top of the chat panel
   - Click on the model selector dropdown
   - You'll see options like:
     - GPT-4 (more powerful, slower)
     - GPT-3.5-turbo (faster, good for simple tasks)
     - Claude (if available)

2. **When to use which model**:
   - **GPT-4**: Complex refactoring, architecture questions, debugging hard problems
   - **GPT-3.5**: Quick questions, simple code generation, explanations

### Workspace Context (Pro Feature)

Use `@workspace` for questions about the entire codebase:

```
@workspace where is the movie API key stored?
@workspace how is local storage used in this app?
@workspace explain the custom hooks
@workspace where are movie ratings calculated?
```

### Slash Commands

In Copilot Chat, try these commands:

- `/explain` - Explain selected code
- `/fix` - Suggest fixes for problems
- `/tests` - Generate tests for code
- `/help` - Show all available commands

### Example Workflow

1. **Select some code in `App.js`** (like the `handleSelectMovie` function)

2. **Right-click** → **Copilot** → **Explain This**

3. **In chat, ask**:
   ```
   Can you make this function more efficient?
   ```

4. **Or ask**:
   ```
   /tests for the handleSelectMovie function
   ```

✅ **Checkpoint**: You can switch between models, use @workspace commands, and use slash commands.

---

## 🎯 Quick Reference

### Common Keyboard Shortcuts

| Action | Windows/Linux | Mac |
|--------|---------------|-----|
| Open Copilot Chat | `Ctrl+Shift+I` | `Cmd+Shift+I` |
| Accept suggestion | `Tab` | `Tab` |
| Reject suggestion | `Esc` | `Esc` |
| Next suggestion | `Alt+]` | `Option+]` |
| Previous suggestion | `Alt+[` | `Option+[` |
| Open terminal | `` Ctrl+` `` | `` Cmd+` `` |
| Command Palette | `Ctrl+Shift+P` | `Cmd+Shift+P` |

### Useful Chat Commands

- `@workspace [question]` - Ask about the entire project
- `/explain` - Explain selected code
- `/fix` - Fix problems in code
- `/tests` - Generate tests
- `/help` - Show help

### Checking Your Setup

Run these checks to verify everything:

1. **Copilot Status**: Click the `><` icon (bottom right) → Should say "enabled"
2. **Model Access**: Open chat → Look for model selector at top
3. **Workspace Features**: Type `@workspace test` in chat → Should work
4. **Extensions**: `Ctrl+Shift+X` → Both Copilot extensions show "Installed"

---

## 🔧 Common Issues and Quick Fixes

### "Copilot is not active"

- Click the Copilot icon (bottom right)
- Click "Sign in"
- Authorize in the browser

### "No model selector in chat"

- Check: https://github.com/settings/copilot
- Make sure your subscription is active
- Sign out and sign back in to VS Code
- Restart VS Code

### "@workspace commands don't work"

- Make sure you have Copilot Pro (not just regular Copilot)
- Update the GitHub Copilot Chat extension
- Reload VS Code window: `Ctrl+Shift+P` → "Developer: Reload Window"

### "npm install failed"

- Make sure Node.js is installed: `node --version`
- Delete `node_modules` and `package-lock.json`
- Run `npm install` again
- Check your internet connection

### For more help

- See [COPILOT_SETUP.md](COPILOT_SETUP.md) for detailed troubleshooting
- Ask in Copilot Chat: "I'm having trouble with [describe issue]"
- Check: https://docs.github.com/en/copilot

---

## 🎓 Next Steps

Now that you have everything set up:

1. **Learn the codebase**:
   ```
   @workspace give me a tour of this movie app code
   @workspace what are the main components?
   @workspace how does the search feature work?
   ```

2. **Make improvements**:
   - Ask Copilot to help add new features
   - Practice refactoring with Copilot's suggestions
   - Use Copilot to write comments and documentation

3. **Explore other files**:
   - `StarRating.js` - Custom rating component
   - `useMovies.js` - Custom hook for fetching movies
   - `useLocalStorageState.js` - Local storage management

4. **Build something new**:
   - Ask: "@workspace how can I add a favorites feature?"
   - Ask: "How can I add movie trailers?"
   - Let Copilot guide you through the implementation!

---

## 📚 Learning Resources

- [GitHub Copilot Docs](https://docs.github.com/en/copilot)
- [VS Code Copilot Guide](https://code.visualstudio.com/docs/editor/github-copilot)
- [React Documentation](https://react.dev/)
- [Create React App Docs](https://create-react-app.dev/)

---

## 🎉 Congratulations!

You now have GitHub Copilot Pro working in VS Code with this movie app project! You're ready to:

- ✅ Get AI-powered code suggestions as you type
- ✅ Ask questions about the codebase with @workspace
- ✅ Switch between different AI models
- ✅ Use chat commands for explanations, fixes, and tests
- ✅ Learn and build faster with AI assistance

Happy coding! 🚀

---

**Need help?** Open Copilot Chat and ask: "I need help with [your issue]" - Copilot is there to help you learn!
