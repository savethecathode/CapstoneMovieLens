# Trouble using GitHub from R Studio on Win10.
The push buttom is not enabled after 


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

git remote add origin <<https-url>>
  
git push -u origin master

Error msg: fatal: protocol 'https' is not supported

git remote add origin <<http-url>>
  
Error msg: fatal: remote origin already exists.

Note: beware of [Ctrl]-V to paste followed by Right-Click-Past**, [Ctrl]-V repends a hidden "^?" to the url, which is invalid, ref.:

https://stackoverflow.com/questions/53988638/git-fatal-protocol-https-is-not-supported


# CapstoneMovieLens

EdX Capstone 
