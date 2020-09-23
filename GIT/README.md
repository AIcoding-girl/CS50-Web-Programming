## GitHub is a website that allows us to store Git repositories remotely on the web.

**Create new repository**  
After creating new repository in Github, in your terminal  
run `git clone <repository url>`

**Create new folder in Github repository**  
You cannot create an empty folder and then add files to that folder, but rather creation of a folder must happen together with adding of at least a single file.
- Go to the folder inside which you want to create another folder
- Click on "New file"
- On the text field for the file name, first write the folder name you want to create
- **Then type / .** This creates a folder
- You can add more folders similarly
- Give the new file a name
- Finally, click "Commit new file".

**Create new file from terminal**  
`touch <file name>`

**Save file to Github from terminal**  
`git add <new file name>`  
`git commit -m "some message"`

   + If you’ve only changed existing files and not created new ones, instead of using `git add .` and then `git commit...`, use  
   + `git commit -am "some message"`  

`git status`  
`git push`

**Update a file from Github through terminal on local computer**  
`git pull`

**Merge conflicts**  
  
Gives a history of all of your commits on that repository  
`git log`

Revert back to a previous commit  
`git reset`  
  
   + `git reset --hard <commit>` reverts your code to exactly how it was after the specified commit. To specify the commit, use the commit hash associated with a commit which can be found using `git log`;  
   + `git reset --hard origin/master` reverts your code to the version currently stored online on Github;

**Open a file with VS Code from terminal**  
`code <file name>`

**While uploading files from other (computer) account, configure your personal GitHub account details**
`
    git config --global user.name "Your Name"
    git config --global user.email you@example.com
`

**Branching** is a method of moving into a new direction when **creating a new feature**, and only combining this new feature with the main part of your code, or the main branch, once you’re finished.  
The branch you are currently looking at is determined by the **HEAD**, which points to one of the two branches. By default, the HEAD is pointed at the master branch, but we can check out other branches as well.  
  
1) `git branch` to see which branch you’re currently working on;  
2) `git checkout -b <new branch name>` to make a new branch;  

`git checkout <branch name>` to switch between branches and commit any changes to each branch;  
When we’re ready to merge our two branches together, we’ll check out the branch we wish to keep (almost always the master branch) and then run the command  
`git merge <other branch name>`. This will be treated similarly to a push or pull, and merge conflicts may appear.  

**More GitHub Features**  

   + **Forking**: As a GitHub user, you have the ability to fork any repository that you have access to, which creates a copy of the repository that you are the owner of. We do this by clicking the “Fork” button in the top-right.  
   + **Pull Requests**  
   + **GitHub Pages**
