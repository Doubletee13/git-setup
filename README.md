# GIT AND GITHUB FOR BEGINNERS

### WHAT IS A VERSION CONTROL?

A version control is a system that tracks and manages changes to files over time

### WHAT IS THE IMPORTANCE OF A VERSION CONTROL?

It helps keep history of changes made to files and it serves as a safe haven to keep these files

### WHAT IS GIT?

Git is a distributed version control used to track changes in codes and collaborate on software development projects

### WHAT IS GITHUB?

Github is a platform that helps developers store,share,and collaborate on code using git.

### DIFFERENCE BETWEEN GIT AND GITHUB?

Git is simply a tool that track changes in code while github is a website that stores git projects online.

### COMPREHENSIVE GIT AND GITHUB SET UP FOR BEGINNERS

Firstly dowload and install git from the url below

>https://git-scm.com/downloads


Then, from the terminal, type the command "git --version" to see the current version of git youhave installed

 
Set up git locally first time only by running the below commands:
>git config --global user.name "Your Name"
>git config --global user.email "your@email.com"


Run the command: 
>git config --list

to confirm your inputted details which are your username and email


Generate a new SSH key pair with the command the below:
>ssh-keygen -t ed25519 -C "email"


Manage your SSH private keys below command:
>eval "$(ssh-agent -s)"

The above is needed so you don't have to type your SSH key passphrase everytime you use the key


Add private key to your running ssh-agent with the below command:
>ssh-add ~/.ssh/id_ed25519


Next is to run the below command:
>cat ~/.ssh/id_ed25519.pub

The above prints out your ssh key which you should copy manually from the terminal


Proceed to creating a Github account here: 
>https://github.com


Sign up with your email and verify it then set up a username and password


Go to settings then to SSH and GPG keys, click "New SSH key", on the title input, give it a name e.gUbuntu Destop and then paste the copied SSH key and finally click "Add SSH key"


You can then proceed to create a repository to push your first project and name it giving no spaces but with underscores and dash e.g "my-first-project"

you can upload your local codes to github by firstly initializing git by running the command:
>cd your-project-folder
>git init

Afterwards, you should add and commit your files by running the commands:
>git add . (adds all files in current working directory)
>git commit -m "My first commit"

Check the states of the files added by running the command:
>git status

Add remote Github repository by running the command:
>git remote add origin git@github.com:your-username/your-repo.git

Push to Github by running the command:
>git push -u origin main (to push to the main branch)
>git push -u origin master(to push to the master branch)


And there! you have fully set up git and github, Congratulations!.
