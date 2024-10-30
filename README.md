- `git init`: initialize current folder as a git repository
- `git clone <url>`: brings the git repo from <url> to current folder
- `git status`: tells us what we need to know about our repository

- `git add <FILE>`: adds <FILE> to the staging area
- `git commit`: open a text editor to write commit message 
  - `git commit -m "MESSAGE"`: writes a MESSAGE as a commit without a text editor

- `git log`: shows the log (history) of our commits
  - `git log --oneline`: shows the shorter oneline commit

- `git diff`: compare current uncommited state with last known git state
  - `git diff --staged`: runs git diff between the staging area and the last known state
- `git diff HEAD~HEAD<NUMBER>`: compares HEAD with commit <NUMBER> ago (relative)
- `git diff <HASH>`: compares HEAD with the commit in <HASH>

- `git restore --source <HASH OR HEAD~>`: restore file to <HASH OR HEAD~>
    - `git checkout <HASH OR HEAD~>`: restores file to <HASH OR HEAD~>
        - `git checkout <HASH OR HEAD~>`: if you forget the file, you end up in detached head state
        - `git checkout master/main`: go back to master/main
        - `git switch master/main`: go back to master/main

- `git remote add <NAME> <URL>`: adds the <URL> as a remote with the name <NAME>
    <NAME> is by convention called `origin`
- `git remote rm <NAME>`: removes the remote called <NAME>
- `git remote -v`: look at all the remotes you have
- `git push <WHERE> <WHAT>`: pushes the <WHAT> branch to <WHERE>
    -`git push origin master`
- `git pull <WHERE> <WHAT>`: pulls the <WHAT> branch in <WHERE> to local computer
