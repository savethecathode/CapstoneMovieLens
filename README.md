# Trouble using GitHub from R Studio on Win10.
The "push"-buttom is not enabled after clicking "commit"-button... 


# Try using Git/GitHub via Git-Bash:
Open R Studio:

File>New Project

Create Project: 

New Directory > New Project

Specify Directory name, and parent dir, BUT do not check box for "Create a git repository"

Open Git-Bash and navigate to dir of Rproj file.

git init

git config --global user.name "githubusername"

git config --global user.email youremaill@gmail.com

git add \<filename\>
  
(git status)

git commit -m "type a msg"

(git status)

git remote add origin \<https-url\>
  
git push -u origin master

Error msg: fatal: protocol 'https' is not supported

git remote add origin \<http-url\>
  
Error msg: fatal: remote origin already exists.

Note: beware of [Ctrl]-V to paste followed by Right-Click-Past**, [Ctrl]-V repends a hidden "^?" to the url, which is invalid, ref.:

https://stackoverflow.com/questions/53988638/git-fatal-protocol-https-is-not-supported


Even when making sure to not use [Ctrl]-V , get error msg:

! [rejected]        master -> master (fetch first)

error: failed to push some refs to 'https://github.com/savethecathode/CapstoneMovieLens.git'

hint: Updates were rejected because the remote contains work that you do not have locally. This is usually caused by another repository pushing to the same ref. You may want to first integrate the remote changes (e.g., 'git pull ...') before pushing again.  See the 'Note about fast-forwards' in 'git push --help' for details.


Try "pull" before "push:

warning: no common commits

remote: Enumerating objects: 39, done.

remote: Counting objects: 100% (39/39), done.

remote: Compressing objects: 100% (38/38), done.

remote: Total 39 (delta 10), reused 0 (delta 0), pack-reused 0

Unpacking objects: 100% (39/39), done.

From https://github.com/savethecathode/CapstoneMovieLens

* branch            master     -> FETCH_HEAD

* [new branch]      master     -> origin/master

fatal: refusing to merge unrelated histories


# CapstoneMovieLens

EdX Capstone 
