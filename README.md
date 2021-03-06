# A Gentle Introduction To Git

## What is Git?

<p>Git is an open-source software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development.</p>


## How do we install Git?
<p>I recommend the following guide for installing Git for your specific operating system.</p>

[Git installation guide by Atlassian](https://www.atlassian.com/git/tutorials/install-git "Install Git")

## What now?

### Let's configure your Git installation to use your name and email!

1. Open your terminal or command prompt.

2. `git config --global user.name "Tony"`

3. `git config --global user.email "tony@email.com"`

4. You can now check your Git configuration using:</br> 
`git config --list`

### Now that we have setup our git Configuration, let's create create a git repository!

1. Create a new folder / directory using a command like:</br> `mkdir tomatoes`

2. Move into the directory that we just created:</br> 
`cd tomatoes`

3. Inside this directory, we will initialize a <b>Git Repository</b> using: </br> `git init` </br>
This command tells Git to create a <b>repository</b> in this folder so that we can monitor all the changes in this repository.

### Woh! We now have our first repository!! Let's add our files to it.

1. Create a new file in the repository called <b>index.html</b> and add [this content to it](./index.html).

2. This is a good time to check the status of out repository using the command:</br> `git status`</br>
This command will show you a list of -Untracked Files- which should contain the index.html file we just added to our repository. <b>Untracked</b> means that git is not currently tracking the changes in this file.

3. We can tell git to start tracking the files using the command: </br> `git add .`</br>
`.` tells git to start tracking all the untracked files.

4. Check the current status of our repository using: </br>
`get status` </br>
We can now see that the previously untracked files are ready to commit.</br>
But, what does it mean to commit?
</br> Commit means saving the current snapshot or version of our repository.
5. We can create a commit using the command: </br>
`git commit -m "Some descriptive and meaningful message"`
</br>
This command will commit our current repository with the given message.
6. This is a good time to check the status of our repository.

## Exercise - 1
Perform the following tasks to check your understanding:

1. Modify the index.html file as indicated by the comment on line 10.
2. Add a new file to the directory, any file.
3. Use the `add` command to track these changes.
4. Commit the you code with a descriptive message (The messages must be useful. Avoid messages like "initial commit" or "made minor changes").

### Great job! Now that we have commited our changes let's create a remote repository on [GitHub](https://github.com).
1. Open GitHub, login and press the `New` button.
</br>
![New Repository][NEW_BUTTON]
</br>
2. Give you repository a name and press the `Create Repository` button.
</br>
![Name the repository][NAME_IT]
</br>
3. Follow the instructions under the `...or push an existing repository from the command line` section.
</br>
![New Repository][PUSH_CODE]
</br>

Done? Refresh the GitHub repository page to check if your code was pushed to the remote repository.</br>
We can now collaborate with our team members!!

## Exercise - 2
Perform the following tasks to check your understanding:
1. Make some changes to index.html
2. `add` these changes to the tracked files.
3. `commit` the changes.
4. Push the changes to the remote repository using: </br>
`git push`
5. Go back to [GitHub](https://www.github.com) to check if your changes were push to the remote repository.

[NAME_IT]: ./assets/name_it.jpeg "Name your repository."

[NEW_BUTTON]: ./assets/new_button.jpeg "Create a new Repository."

[PUSH_CODE]: ./assets/push_existing_repo.jpeg "Push you code to a remote repository"