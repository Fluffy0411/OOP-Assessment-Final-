Part 2: Questions 
Answer these questions in a Markdown file and link it to your README
1.	List three major version control for software engineering. 
GIT, BitBucket, Mercurial
2.	What are the main advantages to using Git in your software development, and how is it useful for game developers. 
Version control – keeping track of all additions, corrections, amendments, merges etc to code  
collaborations  
3.	Define the following terms in relation to Git. Branch, Pull, Push, Repository, Working Copy, Merge
Branch -  A version of the repository that diverges from the main working project. Branches can be a new version of a repository, experimental changes, or personal forks of a repository for users to alter and test changes.
Pull -  If someone has changed code on a separate branch or project and wants it to be reviewed to add to the mater branch, that someone can put in a pull request. A pull happens when adding the changes to the master branch
Push - updates a remote branch with the commits made to the current branch. Literally “pushing” changes onto the remote
Repository - In Git is a central storage location for managing and tracking changes in files and directories. It is a crucial component of the Git version control system ,which enables collaborative development and allows multiple developers to work on a project simultaneously. 
Working Copy - In Git, a working copy refers to the local directory on your computer where you actively make changes to your code.
		Merge - In Git, a merge combines changes from one branch into another branch.
4.	If you are working at a company, which of their policies and procedures might relate to using version control systems such as Git.
Version Control Policy: Companies often have a formal policy that outlines the use of version control systems. This policy may cover aspects such as:
Mandatory use: Requiring all developers to use version control for code management.
Branching strategy: Guidelines on creating branches, merging, and handling feature branches.
Commit conventions: Standards for writing meaningful commit messages.
Code review process: How code changes are reviewed and approved before merging.
Security and Access Control:
Access permissions: Policies regarding who can access specific repositories or branches.
Authentication: Procedures for securely authenticating users when interacting with Git repositories.
Encryption: Ensuring that sensitive data (such as credentials) is not stored in plain text within repositories.
Code of Conduct and Collaboration:
Collaboration guidelines: Encouraging collaboration, respectful communication, and teamwork within version-controlled projects.
Conflict resolution: Procedures for resolving conflicts during merges.
Code ownership: Clarifying who is responsible for maintaining specific parts of the codebase.
Backup and Disaster Recovery:
Backup policy: Ensuring that repositories are regularly backed up to prevent data loss.
Disaster recovery plan: Procedures for recovering from accidental deletions or repository corruption.
Release Management:
Tagging and versioning: Guidelines for tagging releases and managing version numbers.
Changelog creation: Policies on maintaining changelogs to document changes between versions.
Compliance and Legal Considerations:
Licensing: Ensuring that code in repositories complies with open-source licenses or company-specific licenses.
Intellectual property: Procedures for handling contributions from employees or external contributors.
Policies and procedures may vary depending on the company’s size, industry, and development practices. It’s essential to familiarize yourself with your company’s specific guidelines related to version control systems to ensure smooth collaboration and code management

5.	Merge conflicts can occur while using git. List merge tools or diff tools you can use to help you merge and deal with conflicts.
Following are a list of merge tools & diff tools that can be used to help you merge and deal with conflicts whilst using Git.
Merge Tools:
Meld:
A free and open-source visual merge tool available for Linux, Windows, and macOS that
supports three-way merges, allows editing files directly within the tool, provides a simple GUI, supports major version control systems (Git, Mercurial, Subversion, and Bazaar). It provides three-way comparisons, is easy to use and visually appealing. However it has a confusing UI, incomplete auto-merge and inability to compare differently-named files when comparing directories.
P4Merge:
A free visual merge tool available for Windows, macOS, and Linux that provides side-by-side comparison, supports manual code aligning. allows editing files directly. It supports 3-way merges and a customizable UI.
Beyond Compare:
A paid tool available for Windows, macOS, and Linux. It is proprietary software with advanced comparison capabilities, supports folder comparisons and precise editing of compared files.

Diff Tools:
KDiff3:
A free and open-source diff tool for Windows, Linux, and macOS that supports three-way merges, compares whole directory trees, allows editing files directly. It has a customizable UI and diff by character (not just lines). However a confusing GUI, is slow for large files and problems with different line counts.


Visual Studio Code:
Visual Studio Code (VS Code) is a free code editor available for Windows, macOS, and Linux. It has a built-in diff tool, integrates seamlessly with Git & supports extensions for additional functionality. It is lightweight, customizable and widely used by developers.

Notes : Remember to configure your preferred merge and diff tools using Git’s configuration settings. For example:
# Set your preferred merge tool
git config --global merge.tool <tool_name>

# Set your preferred diff tool
git config --global diff.tool <tool_name>

6.	In a merged source code file, how does Git let you know there is a conflict?
In a merged source code file, Git indicates a conflict by inserting special markers directly into the file. These markers highlight the conflicting sections, allowing you to identify and resolve the issues.
Git notifies you of a conflict by:
Conflict Markers:
When you attempt to merge or rebase branches, Git compares the changes made in different branches. If it detects conflicting changes in the same part of a file, it inserts conflict markers.
The conflict markers typically look like this:
<<<<<<< HEAD
// Your changes from the current branch
=======
// Changes from the other branch
>>>>>>> other-branch
The <<<<<<< HEAD, =======, and >>>>>>> other-branch lines indicate the conflicting sections.




7.	What are the steps you can take to resolve Git conflicts?
To resolve Git conflicts following is the task:
a.	Manually edit the file to resolve the conflict.
b.	Decide which changes to keep (from your branch) and which to discard (from the other branch).
c.	Remove the conflict markers and adjust the code as needed.
To resolve Git conflicts following is the process:
a.  Open the conflicted file in a text editor or an integrated development environment (IDE).
		 b.  Locate the conflicting sections marked by the markers.
		 c.  Edit the code to combine the desired changes.
		 d.  Remove the conflict markers.
		 e.  Save the file.
To resolve Git conflicts following is the committing resolution:
a.	After resolving the conflict, stage the modified file using git add.
b.	Commit the changes with a meaningful commit message.
c.	The merge conflict is now resolved.
Notes : Git relies on your judgment to resolve conflicts. Take your time, carefully review the conflicting sections, and ensure that the merged code works correctly. 

8.	What does git revert do, and how can you use it?
The purpose of the git revert command is to remove all the changes a single commit made to your source code repository. Eg if a past commit added a file named index.html to the repo, a git revert on that commit will remove the index.html file from the repo.  
9.	What does git reset do, and how can you use it?
The git reset is used to undo the changes in your working directory and get back to a specific commit while discarding all the commits made after that one. Eg 10 commits are made, using the git reset on the first commit will remove all nine commits taking you back to the first commit stage.
10.	What is the difference between git revert and git reset?
Git revert is a tool for undoing committed changes, while git reset HEAD is for undoing uncommitted changes. Git revert like git checkout has the potential to overwrite files in the working directory, so it will ask you to commit or slash change that would be lost during the revert operation.

11.	True or False: It is okay to commit broken code to the main branch.
	FALSE
12.	True or False: You should commit related changes. For example, fixing two different bugs should produce two separate commits.
	TRUE

13.	Describe what is DevOps, how is it useful for game developers?
DevOps is a collection of best practices and working methods for the software development process whose cumulative goal is to shorten the development life cycle and support practices such as continuous integration , continuous delivery and continuous deployment.
The term DevOps is a combination of Software development and Information Technology Operations sometimes known as IT Operations or ITOps. 
14.	List what tools can be used with DevOps. Give a brief description of each one. (at least 3)
Slack – one platform for team & work, features of Slack work together, cloud based team communication platform , messaging app for businesses that connects people to information they need transforming the way organisations communicate.
Miro – collaboration tool : mind maps, hybrid work, online whiteboard, flowchart
GitHub – developer platform that allows developers to create, store, manage and share code. Uses Git software providing the distributed version

15.	What is CI/CD and how can it be used to automate the game development process?
CI/CD involves the automation process of building, testing, and deploying code changes to different environments, such as development, testing, staging and production. CI/CD can benefit game projects in various ways such as reducing bugs, enhancing collaboration, increasing feedback and enabling faster updates. 
