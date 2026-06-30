#!Bin/Bash
# Git Learning

##What is Git?
- Git is a opensource version control system that designed to track changes in files and coordinate work among multiple people. It saves the snapshots of the file each time we make a push request.
It provide features like - collaborate, version controlling, Offline Capability, Staging Area (Index), snapshot storing model.

## Why Git?
- Git provide a wide range from small to a very large scale snapshot storage service with open-source feature.

##Architecture of Git
Working Directory(workspace) -> Staging Area(Index) -> Local Repository(Commit) -> Remote Repository(Push)


## Working Directory
- Working directory is the first stage of Git it refers to the file where we are editing or making any changes in our local machine.

## Staging Area
- Staging Area is the second step of Git architcture where we put the files to get ready for commit by doing git add at this stage by adding git, an hidden file called .git add in our file in local 
system that will now track each thing of the file from user details, hash code, snapshot or any modification.

## Local Repository
- LOcal repository means the permanently saved snapshot of the file in .git hidden file after we added the file in staging area we done commit where we are ready to push it into remote repo.

## Remote Repository
- Remote Repository means the remote destination where we can add our commited files on like GitHub, Git Bucket, Git etc we can add it instantly after commitor later on because once we commiteed it 
in local repo means it is saved permamntemly in our local system.

we can add a remote repository as an origin in our machine.

## Git Workflow

Working Directory
↓
git add
↓
Staging Area
↓
git commit
↓
Local Repository
↓
git push
↓
GitHub

## Commands Learned

git init - git init initializes the .git hidden folder in our local system to start track each and every changes.  example - git init

git status - It shows the overall status of what we have done, what is tracking or not, if we have any modification or we are up-to-date with the changes or not. examle - git status

git add - Here is the step where we actually give .git file the selective or all files to start tracking with user details, snapshots, hashcodes, modifications in .git file

git commit - BY commited our file we submitted the current unsaved version of our file to the git to save it permantenlty inour local repository. Commit means we are submitting our work to be push 
or reflected on the remote repository immideatly or later on. This step do not require internet connection, git do this without internet/offline.

git log - This command is used to see all the logs or time enteries of the repository it usually saves the each commit with their commit ids where it stores collaborator/users email, their commit 
message, the change made by then on which timestamp

git diff -  We this is the commnad most devops engineers usually use that shows the particullar change made in the file. It shows wheather we added a line/file, deleted it shows both the versions 
in diffrent colors so we do have the idea, like the older one, old lines we previosu ly have are now shows in white, and current changes shows in green with +for adding and -for removing/deleting.

git show

git diff --cached

## Interview Questions
Q1. What is Git?

Answer:

Git is a distributed version control system that tracks changes in source code, enables collaboration among developers, and maintains the complete history of a project.

Q2. What is the difference between git commit and git push?

Answer:

git commit saves a snapshot in the local Git repository.
git push uploads local commits to a remote repository such as GitHub.
Q3. What is the purpose of the staging area?

Answer:

The staging area allows developers to review and selectively choose which changes will be included in the next commit.

Q4. What is the difference between git diff and git diff --cached?

Answer:

git diff compares the working directory with the staging area.
git diff --cached compares the staging area with the last commit.

## What I Learned

- Git stores project history as snapshots rather than tracking every individual file change.
- The `.git` directory is the local Git repository that stores commits and metadata.
- The Git workflow follows: Working Directory → Staging Area → Local Repository → Remote Repository.
- The staging area allows selective commits.
- `git diff` helps review changes before staging.
- `git diff --cached` shows what has already been staged for the next commit.
- Commits are stored locally and do not require an internet connection.
- `git push` is the step that uploads local commits to GitHub.

## Common Mistakes I Made

- Initially, I thought the Git repository meant GitHub. I learned that the Git repository exists locally inside the `.git` directory.
- I thought `git diff` compared commits. I learned that it compares the working directory with the staging area.
- I confused the file mode `100644` with a Git command. I learned that it represents Unix file permissions.


