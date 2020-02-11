# Trouble using GitHub from R Studio on Win10.
The push buttom is not enabled after 


# Try using Git/GitHub via Git-Bash:
git init

git config --global user.name "githubusername"

git config --global user.email youremaill@gmail.com

git add <filename>
  
(git status)

git commit -m "type a msg"
(git status)
git remote add origin <https-url>
git push -u origin master
Error msg: fatal: protocol 'https' is not supported
git remote add origin <http-url>
Error msg: fatal: remote origin already exists.
https://stackoverflow.com/questions/53988638/git-fatal-protocol-https-is-not-supported
Note: beware of [Ctrl]-V to paste followed by Right-Click-Past**, [Ctrl]-V repends a hidden "^?" to the url, which is invalid.

# CapstoneMovieLens

EdX Capstone 
