`git init`: initialize current folder as a git repository
`git clone <url>`: brings the git repo from <url> to current folder
`git status`: tells us what we need to know about our repository

`git add <FILE>`: adds <FILE> to the staging area
`git commit`: open a text editor to write commit message 
  -`git commit -m "MESSAGE"`: writes a MESSAGE as a commit without a text editor

`git log`: shows the log (history) of our commits
  -`git log --oneline`: shows the shorter oneline commit

`git diff`: compare current uncommited state with last known git state
  -`git diff --staged`: runs git diff between the staging area and the last known state
`git diff HEAD~HEAD<NUMBER>`: compares HEAD with commit <NUMBER> ago (relative)
