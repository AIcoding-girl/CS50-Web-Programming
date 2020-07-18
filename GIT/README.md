## GitHub is a website that allows us to store Git repositories remotely on the web.

**Create new repository**  
After creating new repository in Github, in your terminal  
run `git clone <repository url>`

**Create new folder in Github repository**  
You cannot create an empty folder and then add files to that folder, but rather creation of a folder must happen together with adding of at least a single file.
- Go to the folder inside which you want to create another folder
- Click on New file
- On the text field for the file name, first write the folder name you want to create
- **Then type /.** This creates a folder
- You can add more folders similarly
- Give the new file a name
- Finally, click Commit new file.

**Create new file from terminal**  
`touch <file name>`

**Save file to Github from terminal**  
`git add <new file name>`  
`git commit -m "some message"`

   + If you’ve only changed existing files and not created new ones, instead of using git add . and then git commit..., use  
   + `git commit -am "some message"`  

`git status`  
`git push`

**Update a file from Github through terminal on local computer**  
`git pull`

**Merge conflicts**  
Gives a history of all of your commits on that repository  
`git log`

**Open a file with VS Code from terminal**  
`code <file name>`
