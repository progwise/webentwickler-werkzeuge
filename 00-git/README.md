# Scenatio 1: Sharing a project that is stored on your local machine with your friends

Imagine that you have a project that you have been working on for a while and you want to share it with your friends. Then you can use a tool called `git`. Git is a tool that helps people who work together on a project to keep track of all the changes they make to the project, so that everyone knows what is going on and nothing gets lost. 

## Downloading and installing git
You can download and install git from [here](https://git-scm.com/downloads).

## Initializing git on your local repository
Once the Git repository is initialized, then the next step is to initialize git on your local repository. So that you can use git to keep track of the changes you make to your project. To do this, you can open the git terminal and navigate to the folder that contains your project. Then you can use the following command: 

`git init`

## Creating a repository on GitHub

[GitHub](https://github.com/) is a website that allows you to create remote repositories. So that you can share your project with your friends by pushing (uploading) your local repository to it. To do this, you can use the following command to create a new repository on GitHub:

`curl -u 'your-github-username' https://api.github.com/user/repos -d '{"name":"your-repo-name"}'` ?????

Alternatively, you can go the [GitHub](GitHub.com) and create a new repository there. To do this, you can follow the following steps:

1. Click the "+" icon in the top right corner of the page and select "New repository" from the drop-down menu.

2. On the "Create a new repository" page, enter a name for your repository in the "Repository name" field.

3. Optionally, you can add a description for your repository in the "Description" field.

4. Choose whether you want your repository to be public or private.

5. If you want to initialize your repository with a README file, check the box next to "Initialize this repository with a README".

6. You can also choose to add a .gitignore file and a license to your repository. (*gitignore* files are used to tell git which files to ignore, and license files are used to tell people what they can and cannot do with your project.)

7. When you're ready, click the "Create repository" button.

That's it! Your new repository is now created on GitHub. You can now add files and make changes to your repository using Git commands, or you can use GitHub's web interface to upload files and make changes.


## Staging files
Then the next step is to stage the files that you want to commit. Staging means indexing the files the we want to commit and send to the remote server. It means, there might be situations that we do not want to push all the files in our local repository to be pushed to the remote server. Then, in these situations we use the staging with the following command to specify which files want to commit later:

`git add -p`

And then when it asks stage this hunk? We can press ‘y’ to stage the changes in this hunk.

## Branching

If we want switch to a new branch before doing the commit we can use the following command:

`git switch -c <branch-name>`

Also, if we want to know in which branch we are we can use the following command:

`git branch`

or alternatively we can use the following command:

`git status`

## Merging


Moreover, to merge a branch to the current branch in which we are we can use the command:

`git merge  <branch-name>`

## Committing

committing means making a snapshot of the current state of the repo which we want to push to server. Therefore, we should also add a message following the commit command that declares the current state and changes in the local repo. To commit we use the following command:

`git commit -m “commit message”`

## Pushing

Finally, we can push (upload) our repo to the remote server with the following command:

`Git push` 

## Pulling

To sync our local repository with the remote repository, we can use the following command:

`git pull`

# Scenario 2: Cloning a remote repository from GitHub to your local machine

If we want to save a copy of a remote repository from GitHub to our local machine, we should use the `git clone` command. This command will create a new folder in our local machine and will save the remote repository in it. Then, to sync our local repository with the remote repository in the future, we can use the `git pull` command. This command will fetch any changes from the remote repository and merge them into our local repository. If there are any conflicts, we will need to resolve them manually before committing the changes.

In order to save an initial copy of a remote git repository from GitHub we should use the:

`git clone <address to the remote repository>`

The remaining steps are the same as the previous scenario.


### Using `git pull`

To sync our local repository with the remote repository, we can use the following command:

* `git pull`


This command will fetch any changes from the remote repository and merge them into our local repository. If there are any conflicts, we will need to resolve them manually before committing the changes.

[`git pull`](#using-git-pull)



Then, after that for the next times that we want to sync our local repo with the server we should use the following command;

# git add -p or git add -A
What is staging??

# git commit git reset ...


# git push

# git switch and merge locally

# git push again


# merge the PR






* git clone <address to the remote repository>

### <a name="git-pull"></a>git pull

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
