### Git: The Basics


### Introduction

Git is a free open-source version control system. It is used by most developers and programmers these days since this is easy and more efficient than other version control systems. While git stores its data, most of the version control systems these days like Mercurial, TFS, Perforce, and Bazaar are delta-based version control systems. And since git is free, anyone can use it after of course they learn how to. It saves all the code changes and makes them accessible to us. 
In git, we first save an initial version of the code, and over time we keep updating the code which will be tracked. We can see every change we made each time and if we want, we can also go back to the previous version of our code. This is the most required way to keep track of what changes we made to the code from the beginning to date. If you see a bug in your code, you can go back to the previous version, and then since you can see all the changes you made, you can easily track down the bug. Not only for the bugs but sometimes you need to go back because you realize the previous version was better and more efficient than the present one. You can also go back to the beginning, i.e., the start of your code. 
In today’s world, multiple developers merge their work for the best results and git helps to run the same code in a parallel way so that the tracking would be easy. 


### Git Workflow

 ![Workflows](https://miro.medium.com/max/1050/1*PVERoKNe2xxW2_-6uxaAIA.jpeg)


### Git Terms

You might want to familiarize yourself with a few terms before going further on the detailed learning of git. The terms are: - 
•	GitHub: - This is a website that hosts your repositories online. Many people might get confused about this term, but it is just a service that holds your code in repositories. And by its name, we can guess that it is the hub for git. As a matter of fact, this is the largest open-source codebase for all the users around the world. 
1.	Repository: - This is a folder or a place where your project is stored.
2.	Directory: - This is a term we use instead of a folder in the world of programming. 
3.	Terminal: - Also known as command line, this is an interface for your text commands.
4.	CLI: - This is the Command Line Interface.
5.	Cd: - This simply means change directory.
6.	Code Editor: - A code editor is a word processor where you can write codes. The widely used editor these days is Visual Code Studio or VS Code. 
These terms help a lot when you are on your way to learning git in a more detailed way. They are frequently used and when it comes to learning and using git, you have no other options but to learn them by heart.


### Git Commands

Then, when we start git, there are a few major commands which will help you to have a great start. Those git commands are: -
1.	Clone: - Clone brings a repository that is hosted somewhere else into a folder on your local device. You can clone your own project or someone else’s from host websites like GitHub. 
2.	Add: - Add command helps track your files and changes in Git.
3.	Commit: - After you let Git know you have made changes in the file, you will need the Commit command to save that file in git.
4.	Push: - When you commit your changes in git, you will have to push your commits on a remote or web repo. The best example of that repo would be GitHub. 
5.	Pull: This command is used when you want to download changes from the remote repo to your local device. In short, this serves as the opposite of push command. 
6.	Status: To check your repo status
7.	Merge: To merge 
8.	Merge Origin/main: To merge remote repo with the local repo
9.	Init: To initialize a repository
10.	Branch (name): To create a branch
11.	Branch: To list the branches in git
12.	Config: To check your git configurations, to set up your git username, email, and caching credential. 
13.	Checkout: To revert unstaged changes
14.	Log: To see the commit history
15.	Rm: To remove tracked files
16.	Mv: To remove files in git
17.	Log –stat: To see the statistics about changes
18.	Log -p: To see the commit history and the following files changes
19.	Fetch: To fetch remote repo changes
20.	Remote update: To get the contents of remote branches in Git without automatically merging
21.	Branch -r: To check remote branches that git is currently tracking
22.	Merge –abort: To abort a conflicting merge
23.	Remote -v: To view the remote repo URL
24.	Commit --amend: To modify and add changes to the most recent commit
25.	Log Origin/Main: To see the current commit logs of the remote repo

### Some Other Tips and Tricks

There are some notable tips and tricks that can help you will Git. They are: - 
1.	Blank Commits 
Git commit –allow-empty -m “yooo”

2.	Prettify Logs
Git log –pretty=online –graph --decorate

3.	Clean Up local Branches
Git config –global fetch.prune true

4.	File that specifies intentionally untracked files that Git should ignore
.gitignore


## SSH Keys

These are the keys you can generate locally with the SSH-keygen command and then specify the types of encryption, the strength of encryption, and your GitHub email. 
This should look something like this: - 
ssh-keygen -t rsa -b 4096 -c “GitHub email_id”
It will then show the default file for the SSH key. 


## To search the generated key

You can use the “ls | grep testkey” command line in your terminal which will show you your keys. There are two keys: - 

a)	testkey 
It is the private key you need to store sgit ecurely in your local machine. It connects your GitHub since it uses your account via your local machine. 
b)	testkey.pub
It is the public key you upload on your GitHub interface. It can be generated only with the help of your private key. It can be printed out with the command line “cat testkey.pub”. You can add the key by copying it from there to the GitHub account you have and then your local git command-line interface will know about the key you generated. 

Git is nothing but a system to help you track your code from time to time without losing what you did earlier and with a provision that lets you improvise the code according to your need. 