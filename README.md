# datafun-03-analytics

##CC3.3: Start a Project in GitHub & Clone it Down

Git keeps our code in the cloud (GitHub) and on our machine in sync. It's common to use powerful tools on our machine while we work on confidential data. Then, we push our code to a remote repo for sharing and collaboration.

Git is the software system that manages this. It tracks the evolving code and keeps a full history. 

Terms to know
remote - the cloud repository (e.g., the project folder in GitHub)
origin - a short alias for the URL of the remote repo
URL - the web address of our project folder on GitHub
root folder - the main project folder (both in the cloud and on our machine)
. - dot - means "this folder right here"
.. - two dots, no space between them means the parent folder just above this folder (e.g. Documents)
local repo - a Git-managed folder on your machine.
Different Workflow Options
Since our code lives in two places, there's two ways we can start (locally on our machine or in the cloud/GitHub). We want you to know Option 1 exists, but it takes more git skills, so we don't recommend it. Use the easier Option 2 instead. 

 

##Option 1: Start Project Locally (More Git Skills Required)
Start a New Project Locally on Your Machine. 

Note: Starting on your machine uses an old name for the default branch "master" and we must set it to the new GitHub default branch name "main". Throughout the course, we work only in the "main" branch. 

Open a terminal in your project directory.
Create a new directory named "datafun-03-temp" (or a name of your choice).
Change your working directory (use the cd command) to "datafun-03-temp."
Initialize a Git repository in this directory by opening git bash or Terminal or PowerShell and running: git init
Notice how it adds a .git folder to the project folder.
Take a screenshot showing your terminal with the commands used to create the local repository.
Optional. If we wanted to use this method, we'd complete using something like the following:

Create a README.md file in the project repository folder. 
Run the following commands (use your GitHub url):
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/denisecase/datafun-03-spec.git
git push -u origin main
We won't continue to use this repo - it was just for practice. We want a repo in sync with our remote GitHub repo. We'll do this the EASY way. 

##Option 2: Start Project in GitHub (Easy)
The easier way is to start a project in GitHub, with a default README.md and clone it down. 

Go to GitHub and create a new GitHub repo in your browser for Project 3 (use datafun-03-analytics or whatever the specification requires). Be sure to add a default README.md when you first create the repository - it makes the easiest workflow. If you forget, delete the empty repo and start again. 

Copy the URL of your new GitHub repo into your clipboard (CTRL+A, then CTRL+C, or CMD if on Mac).

Open a Git Bash, Terminal, or PowerShell terminal in your Documents folder (the parent folder of where you want your repo) and type:  git clone paste_your_repo_URL_here

My command might look like this - yours should use your GitHub username instead of denisecase:

git clone https://github.com/denisecase/datafun-03-analytics
Cloning does several things

When you clone a Git repository from a remote source, such as GitHub, it performs several actions to set up a local copy of the repository on your machine:

Copies Repository Contents: Cloning copies all the files and directories from the remote repository to your local machine. This ensures that you have an exact replica of the remote repository's contents.

Initializes a Git Repository: After copying the files, Git initializes a new local repository in the directory where you cloned the repository. This means that Git starts tracking changes and version history for these files locally.

Sets Up Remote Alias (origin): Git sets up a remote alias called "origin" by default. This alias points to the URL of the remote repository you cloned from. It allows you to interact with the remote repository easily, such as pushing changes to it.

Retrieves Commit History: Git also fetches the commit history of the remote repository. This history includes all the commits, branches, and tags made in the remote repository. Your local Git repository will be aware of these details.

Recommendation: Use Option 2 Throughout the Course
See why we recommend this method? Git clone takes care of many things for us. When we start in GitHub and clone down, we set the default branch to main and everything works. 

If you start with git init on your machine, it uses the old "master" branch and you need more git skills. 

Use the recommended Option 2 process (git clone) to avoid "master" branch errors - we recommend using Option 2 throughout the course (or until you decide you want to learn git branching.)

Practice: Clone An Interesting Project in VS Code
Now that you've cloned your own project, find another interesting project to steal - I mean - clone - from GitHub using VS Code. 

