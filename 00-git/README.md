in order to save an initial copy of a remote git repository from GitHub we should use the:

# git clone or git init ?


# git add -p or git add -A
What is staging??

# git commit git reset ...


# git push

# git switch and merge locally

# git push again


# merge the PR






* git clone <address to the remote repository>

Then, after that for the next times that we want to sync our local repo with the server we should use the following command;
* git pull

Staging means indexing the files the we want to commit and send to the remote server. It means, there might be situations that we do not want to push all the files in our local repository to be pushed to the remote server. Then, in these situations we use the staging with the following command to specify which files want to commit later:

* git add -p

And then when it asks stage this hunk? We can press ‘y’ to stage the changes in this hunk.



If we want switch to a new branch before doing the commit we can use the following command:

* git switch -c <branch-name>

Also, if we want to know in which branch we are we can use the following command:

* git branch


Then, we should commit the files want to push to server. Commit, means making a snapshot of the current state of the repo which we want to push to server. Therefore, we should also add a message following the commit command that declares the current state and changes in the local repo. To commit we use the following command: 

* git commit -m “commit message”

And finally we can push our repo to the remote server with the following command: 

* Git push
