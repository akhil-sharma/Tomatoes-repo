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
This command will show you a list of -Untracked Files- which should contain the index.html file we just added to our repository. <b>Untracked</b> means  