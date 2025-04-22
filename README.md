<div align='center'>
 <img style="width:100%" src="https://capsule-render.vercel.app/api?type=soft&height=200&color=FFFFFF&text=How%20to%20use%20Git&fontSize=50&fontAlign=50&strokeWidth=0&desc=Learn%20how%20to%20use%20git%20in%20all%20your%20projects&descAlignY=80&stroke=000000">
</div>

<h2>ABOUT GIT</h2>
<p>Git is a distributed version control system that helps developers manage and track changes in their code. It allows teams to collaborate efficiently, maintain code history, and experiment with new features without affecting the main project. Git is an essential tool in modern software development workflows.</p>

<h2>WHY USE GIT?</h2>
<ul>
  <li><strong>Collaboration:</strong> Git enables multiple developers to work on the same project without conflicts, streamlining teamwork.</li>
  <li><strong>Version History:</strong> Every change is tracked, allowing developers to revert to previous versions and understand the evolution of the code.</li>
  <li><strong>Branching:</strong> Developers can create isolated branches to test new features or fix bugs without disrupting the main codebase.</li>
  <li><strong>Open Source & Widely Used:</strong> Git is free, actively maintained, and used by millions of developers and companies around the world.</li>
</ul>

<h2>INSTALLING GIT</h2>
<p>Getting started with Git is simple. It can be installed on all major operating systems, including Windows, macOS, and Linux. Follow the steps below to install Git on your machine:</p>
<ul>
  <li><strong>Windows:</strong> Download the installer from <a href="https://git-scm.com">git-scm.com</a> and follow the setup instructions.</li>
  <li><strong>macOS:</strong> Use Homebrew with the command <code>brew install git</code>, or download it directly from the official site.</li>
  <li><strong>Linux:</strong> Use your package manager, for example: <code>sudo apt install git</code> (Ubuntu/Debian).</li>
  <li><strong>Verify Installation:</strong> After installing, run <code>git -v</code> in the terminal to confirm Git is correctly installed.</li>
</ul>
<p><em>Example output:</em> <code>git version 2.48.1.windows.1</code></p>

<h2>HEAD, STAGING AREA AND WORKING DIRECTORY</h2>
<p>Git works with three main areas:</p>
<ul>
  <li><strong>HEAD:</strong> Refers to the latest commit in the current branch. It acts as a reference for the most recent state of your project.</li>
  <li><strong>Staging Area:</strong> The area where files are placed before committing. It's like a "preview" of what will be added to the commit.</li>
  <li><strong>Working Directory:</strong> The actual directory where files are modified, added, or deleted. This is where active development occurs.</li>
</ul>

## 🚀 GIT COMMANDS CHEAT SHEET

Git is a powerful version control system that helps developers track code changes, collaborate efficiently, and manage project history. Below is a categorized list of essential and advanced Git commands.

---

### 🔰 INITIALIZATION & CONFIGURATION

- `git init` – Initialize a new Git repository.
- `git config` – Set Git configuration values.
- `git config --global user.name "Your Name"` – Set your global username.
- `git config --global user.email "you@example.com"` – Set your global email.
- `git config --list` – View current Git configuration.

---

### 📦 CLONING & REMOTES

- `git clone <url>` – Clone a remote repository.
- `git remote` – List remote repositories.
- `git remote add origin <url>` – Add a new remote.
- `git remote -v` – Show remote URLs.
- `git fetch` – Fetch changes from remote (no merge).
- `git pull` – Fetch and merge remote changes.
- `git push` – Push commits to remote.
- `git push -u origin main` – Push and set upstream.

---

### 🧾 STATUS, HISTORY & LOGS

- `git status` – Show current changes and staging info.
- `git log` – View commit history.
- `git show` – Show details of a specific commit.
- `git diff` – View changes between commits or branches.
- `git blame <file>` – Show who changed each line in a file.
- `git shortlog` – Summarize commits per contributor.

---

### 🗂️ STAGING & COMMITTING

- `git add <file>` – Stage specific file.
- `git add .` – Stage all modified and new files.
- `git reset <file>` – Unstage a file.
- `git commit -m "message"` – Commit changes with a message.
- `git commit -am "message"` – Stage and commit tracked files.
- `git commit --amend --no-edit` – Edit the last commit.

---

### 🌿 BRANCHING

- `git branch` – List branches.
- `git branch <name>` – Create a new branch.
- `git checkout <name>` – Switch to a branch.
- `git switch <name>` – Switch to a branch (modern alternative).
- `git switch -c <name>` – Create and switch to a new branch.
- `git merge <name>` – Merge another branch into the current one.
- `git rebase <branch>` – Rebase changes onto a different base.

---

### 🧹 UNDO & FIXES

- `git reset` – Unstage or undo commits.
- `git reset --hard HEAD` – Reset to the last commit, discarding all changes.
- `git clean -f` – Remove untracked files.
- `git revert <commit>` – Revert a commit with a new commit.
- `git stash` – Save current changes temporarily.
- `git stash pop` – Restore stashed changes.
- `git cherry-pick <commit>` – Apply a specific commit on the current branch.

---

### 🔍 SEARCH & NAVIGATION

- `git grep "<pattern>"` – Search text across your repository.
- `git show <commit>` – Show details of a commit.
- `git describe` – Describe a commit using the most recent tag.

---

### 🧪 TAGS

- `git tag` – List tags.
- `git tag <name>` – Create a tag.
- `git tag -a <name> -m "message"` – Create an annotated tag.
- `git push origin <tag>` – Push tag to remote.

---

### 🧠 ADVANCED

- `git reflog` – View reference logs (even deleted commits).
- `git bisect` – Find the commit that introduced a bug.
- `git archive` – Create a zip/tar archive of the repository.
- `git submodule` – Manage nested repositories inside your project.

<h2>ABOUT .gitignore</h2>
<p>The <code>.gitignore</code> file is used to tell Git which files or directories to ignore in a project. This is important because certain files, such as log files, build outputs, or sensitive data (e.g., passwords), do not need to be tracked or committed to version control. Using a <code>.gitignore</code> file helps keep the repository clean and focused only on the files necessary for the project.</p>
<ul>
  <li><strong>Exclude unnecessary files:</strong> You can add files like <code>*.log</code>, <code>*.tmp</code>, or <code>node_modules/</code> to ignore unnecessary files that are specific to your development environment.</li>
  <li><strong>Customizable:</strong> The <code>.gitignore</code> file is highly customizable to fit the needs of different programming languages, frameworks, or environments.</li>
  <li><strong>Easy to maintain:</strong> Once set up, you don’t need to worry about accidentally adding files that shouldn't be tracked by Git.</li>
  <li><strong>Common .gitignore examples:</strong> For example, for a Node.js project, you might add <code>node_modules/</code> to <code>.gitignore</code> to avoid committing dependencies that can be installed via <code>npm</code>.</li>
</ul>
<p>Here’s an example of what you might include in a typical <code>.gitignore</code> file:</p>
<pre><code>*.log
*.tmp
/node_modules
backups/</code></pre>
<p>To create a <code>.gitignore</code> file, simply create a new text file named <code>.gitignore</code> in the root directory of your project and list the files or folders to exclude.</p>





<footer align="center">
 <img style="width:100%" src="https://capsule-render.vercel.app/api?type=soft&height=20&color=FFFFFF&fontSize=50&fontAlign=50&strokeWidth=0&descAlignY=80&stroke=000000&reversal=false&section=footer">
</footer>
