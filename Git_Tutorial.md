
# GIT & GITHUB
## What is GIT ?
- Distributed version control system (VCS)
- Control versions of files.

## Features ?
- Tracking changes of files.
- Backup and restore: can revert back to previous changes.
- collaboration : multiple people work together
- branching & merging

## Instllation
- default on mac/linux
- using with VS code

## config user
`# git config --global user.name "Varun Sharma"`
`# git config --global user.email "er.varunsharma89@gmail.com"`
`# git config --list`
credential.helper=osxkeychain
init.defaultbranch=main
user.name=Varun Sharma
user.email=er.varunsharma89@gmail.com

## Creating Repository.
- Local directory to track is repo.
# git init              // initiate the current directory as repo.
# git status            // check the current status 
# git add <file>
# git commit -m "description"       
# git log               // to see logging

What is GIT commit ?
- captures snapshot of project's current stage. (ready state to save state)

++ Commands ++

# git diff                              // to see diffrence between current and stage files.
# git show <version id> <file_path>     // TO see old version file (single file)

Case 1: Changes made by-mistake in file only (no git add yet) and want to restore the last working version.
# git restore <file> or 
# git restore .

Case 2: changes made after git add and want to restore the last working version.
# git diff --cached                     // check the changes in staging area.
# git restore --staged <file>
# git restore <file>

Case 3: Changes to staging and updated the file.
# git restore --worktree index.html

Case 4: Commit by mistake or in wrong file, want to move pointer (header) to last working version.
# git reset --soft HEAD^
# git reset --hard HEAD^

++ Git log options
# git log -2                            // see last 2 logs
# git log -p -2                         // detailed logs for last 2 logs
# git log --stat                        // see stats of logs
# git log --pretty=oneline              // shorter logs
# git log --pretty=format:"%h - %an, %ar:%s"        // customized logs
# git log --grep="<text>"               // grep from subject line
# git log --since="YYYY-MM-MM"          // logs since date 
# git log --author="varun"              // logs by author


++ Remote Repository
Version of the local Repository saved on cloud or remote server.

++ GITHUB ++
Remote Repository cloud hosting for your codes/files/data.

# git remote -v                         // to check remote repo
# git push                              // To push data to remote repo after local commit

++ Cloning 
# git clone <http>                      // to clone repo from GITHUB
# git pull                              // to pull updated version of repo from GITHUB

++ Branching & Merging
Branching used to enhance the code without effecting the original code or branch until tested.
After testing, the branches can be merge into main code.

# git branch                            // To check current branches.
# git branch design                     // To create new branch
# git checkout design                   // switched or change to another branch
After updating code in 'design' branch, it can be merge to 'main' branch.
# git checkout main 
# git merge design                      // merge 'design' into 'main' branch

++ Merge conflicts 
When multiple branches wants to merge with 'main' bracnh, only one is accepted.

++ Fork & merge
another user can fork (copy) the repo to enhance the codes and request (push) the update request.
owner can review the merge/pull request and take action.
 
 ++ gitignore
 create a file with list of files to ignore the commit.

 ++ git clean
 # git clean                            // to remove untagged files.

 ++ git tags
 # git tag -a lat_verison -m "latest version"


 # GITLAB
 
