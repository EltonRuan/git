<div align='center'>
 <img style="width:100%" src="https://capsule-render.vercel.app/api?type=soft&height=200&color=FFFFFF&text=How%20to%20use%20Git&fontSize=50&fontAlign=50&strokeWidth=0&desc=Learn%20how%20to%20use%20git%20in%20all%20your%20projects&descAlignY=80&stroke=000000">
</div>

<div align="center" style="margin-bottom: 20px;">
  <h2>🔗 NAVIGATION </h2>

  <a href="#about-git">ABOUT GIT</a> |
  <a href="#why-use-git">WHY USE GIT</a> |
  <a href="#installing-git">INSTALLING GIT</a> |
  <a href="#head-staging-area-and-working-directory">HEAD, STAGING & WORKING DIRECTORY</a> |
  <a href="#git-commands-cheat-sheet">GIT COMMANDS</a> |
  <a href="#about-gitignore">ABOUT .GITIGNORE</a> |
  <a href="#git-tips-for-effective-usage">GIT TIPS</a> |
  <a href="#final-considerations">FINAL CONSIDERATIONS</a>
</div>

## ABOUT GIT
<p>Git is a distributed version control system that helps developers manage and track changes in their code. It allows teams to collaborate efficiently, maintain code history, and experiment with new features without affecting the main project. Git is an essential tool in modern software development workflows.</p>
<img src="https://skillicons.dev/icons?i=git,&perline=20" />

## WHY USE GIT?
<ul>
  <li><strong>Collaboration:</strong> Git enables multiple developers to work on the same project without conflicts, streamlining teamwork.</li>
  <li><strong>Version History:</strong> Every change is tracked, allowing developers to revert to previous versions and understand the evolution of the code.</li>
  <li><strong>Branching:</strong> Developers can create isolated branches to test new features or fix bugs without disrupting the main codebase.</li>
  <li><strong>Open Source & Widely Used:</strong> Git is free, actively maintained, and used by millions of developers and companies around the world.</li>
</ul>

## INSTALLING GIT
<p>Getting started with Git is simple. It can be installed on all major operating systems, including Windows, macOS, and Linux. Follow the steps below to install Git on your machine:</p>
<ul>
  <li><strong>Windows:</strong> Download the installer from <a href="https://git-scm.com">git-scm.com</a> and follow the setup instructions.</li>
  <li><strong>macOS:</strong> Use Homebrew with the command <code>brew install git</code>, or download it directly from the official site.</li>
  <li><strong>Linux:</strong> Use your package manager, for example: <code>sudo apt install git</code> (Ubuntu/Debian).</li>
  <li><strong>Verify Installation:</strong> After installing, run <code>git -v</code> in the terminal to confirm Git is correctly installed.</li>
</ul>
<p><em>Example output:</em> <code>git version 2.48.1.windows.1</code></p>

## HEAD, STAGING AREA AND WORKING DIRECTORY
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

## ABOUT .gitignore
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

## Git Tips for Effective Usage
<p>Here are some helpful tips to make the most out of Git:</p>
<ul>
  <li><strong>Commit Frequently:</strong> Make small, frequent commits rather than large, infrequent ones. This makes it easier to track changes, understand the history, and resolve conflicts.</li>
  <li><strong>Write Descriptive Commit Messages:</strong> A clear and descriptive commit message helps others (and your future self) understand the purpose of the changes. A good format to follow is: <code>git commit -m "Fixed bug in user login"</code>.</li>
  <li><strong>Use Branches for New Features:</strong> Always create a new branch for new features or bug fixes to avoid messing with the main branch. This helps in maintaining a clean, stable main codebase.</li>
  <li><strong>Stay Synced with Remote:</strong> Run <code>git pull</code> regularly to keep your local repository up-to-date with the remote repository. This minimizes merge conflicts.</li>
  <li><strong>Use .gitignore Wisely:</strong> Make sure to add files you don't want to track (like log files, build directories, and personal configurations) to your <code>.gitignore</code> to avoid unnecessary clutter in your repo.</li>
  <li><strong>Leverage Git Tags for Releases:</strong> Use Git tags to mark specific points in your project’s history, such as releases. This allows you to easily refer to a particular version in the future with <code>git tag <tagname></code>.</li>
  <li><strong>Review Changes Before Committing:</strong> Use <code>git diff</code> to review the changes made before committing. This ensures that only the intended modifications are staged.</li>
  <li><strong>Keep Your Branches Short-Lived:</strong> Don't let feature branches get too outdated. Try to merge them back to the main branch as soon as the feature is complete to avoid long-running branches and difficult merges.</li>
  <li><strong>Use Git Aliases:</strong> If you frequently use certain Git commands, you can create aliases to make them shorter and easier to remember. For example, you can set up <code>git config --global alias.st status</code> to use <code>git st</code> instead of <code>git status</code>.</li>
  <li><strong>Practice Safe Merging:</strong> When merging, ensure you’re merging from the correct branch and be mindful of potential conflicts. It’s helpful to do <code>git fetch</code> and <code>git rebase</code> before merging to keep your history clean.</li>
</ul>

## Final Considerations
<p>This guide was created to help facilitate the learning process and provide a clear, concise understanding of Git for developers of all levels. Whether you're just starting out or looking to refine your knowledge, these tips and commands should serve as a solid foundation to work more efficiently with Git.</p>
<p>Feel free to explore, experiment, and apply these techniques in your projects. The power of version control is in your hands, and mastering Git will undoubtedly make you a more effective developer, capable of collaborating and managing code with ease.</p>
<p>Don't hesitate to refer back to this material as needed, and always keep learning. Git is an essential tool for every developer, and continuous practice is the best way to improve your skills!</p>
<p>Good luck, and happy coding!</p>
<br><br>
<p><strong>© 2025 EltonRuan. All rights reserved.</strong></p>

<footer align="center">
 <img style="width:100%" src="https://capsule-render.vercel.app/api?type=soft&height=20&color=FFFFFF&fontSize=50&fontAlign=50&strokeWidth=0&descAlignY=80&stroke=000000&reversal=false&section=footer">
</footer>
