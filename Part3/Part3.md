 
Part 3: Git Manual
Answer these questions in a Markdown file and link it to your README
Imagine you are working at a game studio, and they want you to help with installing Git. 
1.	Write instructions on installing git on a windows system. Making sure to include
a.	What are the requirements to install Git on a system.
b.	If you had issues installing Git the workplace, give instructions on who you could you enquire about the installation disruption. 
Instructions for installing Git on a Windows system:
Requirements:
Windows System or Windows VPS Compatible with Git:
Ensure that your system is running Windows (e.g., Windows 10, Windows 11).
Administrative privileges are required for installation.
Access to a Command-Line Interface:
You’ll need access to a command-line tool such as CMD or PowerShell. (Umm, what about me –  Gitbash?? Mentioned further on.)
Preferred Text Editor:
Choose a text editor for coding (optional but recommended).
Installation Steps:
Check if Git is Already Installed:
Open the terminal application (CMD or PowerShell). 
Type git version.
If Git is installed, it will display the version. Otherwise, proceed to the next step.
Install Git Using GitHub Desktop (Recommended):
Download and install GitHub Desktop.
GitHub Desktop includes Git and provides a user-friendly GUI for collaboration.
Install Git Manually:
Navigate to the latest Git for Windows installer.
Download the latest version.
Run the installer and follow the instructions in the Git Setup wizard screen.
Choose installation options (components, shortcuts, etc.).
Open the Windows command prompt (or Git Bash if you opted not to use the standard Git Windows Command Prompt during installation).
Type git version to verify that Git was installed.
Troubleshooting Installation Issues:
If the installation gets stuck:  (Yep did I get stuck!)
Open Task Manager.
Select the Git installation process and end the task.
Verify if Git is working by typing git version.
If you encounter issues, consider creating a new admin account or installing Git on a virtual machine to test the installation. (Thank goodness it didn’t get to this stage!)
Adding Git to the PATH (Optional):
If Git is not automatically added to the system PATH:
Locate the Git installation directory (e.g., C:\\Program Files\\Git\\cmd).
Add this directory to the system PATH environment variable.
Restart your command prompt or any application where you want to run Git to reflect the changes.
Verify Git Installation:
Open the terminal (CMD or PowerShell).
Type git version to ensure Git is installed and working correctly.
That’s it! You now have Git installed on your Windows system. You can start using Git for version control and collaboration on your projects.
If you encounter any issues during installation, feel free to ask for further assistance or enquire within your workplace for guidance (ie ask a real ICT technical support department for help) 







2.	Do research on some principles/techniques of industry standard best practices creating and working with repositories and branches in Git. 
a.	List the most important principles/techniques for creating and working with repositories
b.	List the most important principles/techniques for creating and working with branches
Principles and Techniques for Creating and Working with Repositories:
Initialize a Repository:
Use git init to create a new Git repository in your project directory. This initializes a .git subdirectory where Git stores its configuration and version history.
Cloning Existing Repositories:
Use git clone <repo_url> to create a local copy of an existing remote repository. Cloning is a one-time operation and provides you with a working copy for development.
README Files:
Always include a README.md file in your repository. It serves as documentation for your project, explaining its purpose, setup instructions, and usage.
Branching Strategies:
Choose a branching strategy that suits your project needs (e.g., Trunk-Based Development, Feature Branching, Git Flow). Each strategy has advantages and trade-offs.
Git Ignore:
Create a .gitignore file to specify files and directories that Git should ignore (e.g., build artifacts, temporary files, IDE-specific files).
Commit Frequently:
Make small, focused commits with meaningful messages. Frequent commits help track progress and simplify code reviews.
Avoid Binary Blobs:
Git is designed for text files. Avoid committing binary files (e.g., images, compiled executables) directly to the repository. Use Git LFS for large binary files.
Principles and Techniques for Creating and Working with Branches:
Branch Creation:
Create branches for different features, bug fixes, or experiments. Use git checkout -b <branch_name> to create and switch to a new branch.
Feature Branches:
Use feature branches to isolate work on specific features or user stories. Merge them back into the main branch (e.g., master or main) when complete.
Hotfix Branches:
For critical issues in production, create hotfix branches. Fix the issue, test it, and merge the hotfix back into the production branch.
Branch Naming Conventions:
Follow consistent naming conventions for branches (e.g., feature/add-login, bugfix/fix-bug-123).
Switching Between Branches:
Use git checkout <branch_name> to switch between branches. Ensure a clean working state before switching.
Merging and Rebasing:
Merge branches using git merge. Consider rebasing (git rebase) to maintain a linear commit history.
Pull Requests (PRs):
If using a collaborative platform (e.g., GitHub, GitLab), create PRs for code review and discussion before merging branches.
Git can be a powerful tool, and understanding these principles can help manage repositories and branches effectively. 


3.	List the steps in a Git workflow that the team should follow when working on projects.
		1. Create a repository
		2. Create a new branch, Use a separate branch for each new feature or issue worked on
 		3. Update, add, Commit & Push changes
		4. Push feature branch to remote
		5. Resolve feedback
		6. Merge pull requests
