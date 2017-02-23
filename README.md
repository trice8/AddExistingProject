# Trying to add existing project to githubHub.

1) Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

2) Open Git Bash.

3) Change the current working directory to your local project.

4) Initialize the local directory as a Git repository.

``
$ git init
``

5) Add the files in your new local repository. This stages them for the first commit.

```
// Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
$ git add .
```

6) Commit the files that you've staged in your local repository.

```
// Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
$git commit -m "First commit"
```

7) At the top of your GitHub repository's Quick Setup page, click 'Copy to clipboard' to copy the remote repository URL.

8) In the Command prompt, add the URL for the remote repository where your local repository will be pushed.

```
// Sets the new remote
$ git remote add origin remote repository URL

// Verifies the new remote URL
$ git remote -v
```

9) Push the changes in your local repository to GitHub.

```
// Pushes the changes in your local repository up to the remote repository you specified as the origin
$ git push origin master
```

10) Make existing branch trak remote branch

```
// git branch --set-upstream-to=/< remote>/< branch> < localbranch>
$ git branch --set-upstream-to=origin/foo
```

# Links
https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/

http://stackoverflow.com/questions/520650/make-an-existing-git-branch-track-a-remote-branch
