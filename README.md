# JupyterLab Learning Example
Uses Python, JupyterLab and git as examples to learn how to use the tools in classwork.

## Installation
1. Use the green code button above to get the link to the code.
1. Make sure HTTPS is underlined in red.
2. Click on the two boxes at the end of the "*https:...*" line.
3. Open *Git Bash* (Windows) or *Terminal* (macOS). **From here on, the application window will be called the command line interface (CLI).** 
4. In Explorer (Windows) or Finder (macOS), go to a base folder of your choice, such as "*My Documents*" or "*Documents*" and drag the icon of the folder to your CLI. This is an easy way to open that folder in the CLI.
5. In the CLI, type "*pwd*" to ensure you are in the right folder, it needs to end with "*My Documents*" or "*Documents*".
6. In the CLI, enter "git clone " (make sure there is a space after the "e"), and *paste* the contents from step 2 above.
7. The line will look something like this (see below) and press return.
	```bash
	git clone https://github.com/lkoepsel/jupyterlab.git
	```
9. Hit return, this will create a new folder called "*jupyterlab*" on your computer.
10. Use the application *jupyterlab* to open the folder.

## Additional Git Commands Required
Git will want to know who you are and your email address, so it can identify you as the author of your changes. This information doesn't go anywhere, it simply is part of the repository. These two commands will need to be executed prior to using the *Fundamental Git commands*.

```
git config --global user.name "MY Name"
git config --global user.email "myname@mail.com"
```

## Fundamental Git commands
1. Once you made some changes and wish to add the changes to your repository, you will need to *add* them.
	```
	git add -A
	```
2. When the changes are **added**, they are now known as **staged**, which is an iterim step in *git*. It is where *git* knows you have changed the file and it needs to account for it in any operation. To move from **staged** to **committed**, you will need to *commit*. **Be sure to change the text "*message*" to a short appropriate message describing what changed.**
	```
	git commit -m "message"
	```
3. To be safe, it is best to then copy those changes to your own repository in the cloud. This can be on GitHub, GitLab or BitBucket. This is known as a **push** and uses *push name* to accomplish. **Note: This step requires you to have setup already, an account on one of the repositories (GitHub, GitLab or BitBucket).**
	```
	git push origin
	```

Now your changes have been logged and you are able to continue knowing you may go back in time, if you have a difficult to solve error in your code!

One more very helpful command is `git status`, at any point in time if you are confused as to what changes exist on your repository, use this command. As in:

	```
	git status
	On branch main
	Your branch is up to date with 'origin/main'.

	Changes not staged for commit:
  		(use "git add <file>..." to update what will be committed)
  		(use "git restore <file>..." to discard changes in working directory)
			modified:   README.md

	no changes added to commit (use "git add" and/or "git commit -a")
	```
## Links
* [Python 3.8 Tutorial](https://docs.python.org/3.8/tutorial/index.html)
* [Markdown Reference](https://commonmark.org/help/)
