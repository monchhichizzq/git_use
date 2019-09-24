# git_use
Git

Git and GitHub

	Seting the SSH protocol for local Git to communicate with GitHub
	
	• Store the public and private keys in the .ssh directory of the user directory
	• cd ~/.ssh/ (if .ssh doesn't exist, create a new one by mkdir ~/.ssh)
	• Configure the global name and email, here is the name and email of your github
	• git config --global user.name 'Zeqi'
	• git config --global user.email 'miaomiaochaoshuai@gmail.com'
	• generate the key
	• ssh-keygen -t rsa -C 'miaomiaochaoshuai@gmail.com'
	• Press Enter three times in succession, the password set here is empty, and the key is created.
	• Finally got two files: 
	• id_rsa and id_rsa.pub
	• Open the Admin directory and enter the .ssh folder. Open the id_rsa.pub with Notepad and copy the contents to your github or bitbucket ssh settings.     C:\Users\....\.ssh
	• Open id_rsa.pub and copy all
	• Github/ settings/ SSH and GPG keys -- New SSH key
	• Test
	• ssh git@github.com
	• Success message:  
	• “Hi lsyz0021! You've successfully authenticated, but GitHub does not provide shel l access.”
	• Begin to use github


	Connecting local and remote repository on github
	
	• Download and install git  https://git-scm.com/

	• Create a folder 'Gitfirst'
	• cd '..\Gitfirst'


	• user name setting - git config --global user.name 'Zeqi'
				□  - git config --global user.email 'miaomiaochaoshuai@gmail.com'  
	• verification            - git config user.name

	• create  a repository - git init
	for mac: ls -a (visualize the git repository)
	• Connect local repository and github
	git remote add origin https://github.com/monchhichizzq/Deep_learning-Ensemble_learning.git (HTTPS)
	
	• add new script - touch 1.py
	• view - git status

	• The file '1.py'  hasn't been added to the repository, please follow those steps to complete it:
	• git add 1.py / git add*
	• git commit -m 'first_commit'
	• In this way , local changes have taken effect

	• We need to push the local repository to the remote cloud
	• git push -u origin master


	
	Processing the existing repository on Github (Pull Requests)
	
	• Search for the existing repository on Github
	• Click Fork (copy the existing repository to your Github)
	• Click  'edit this file' and submit
	• Your blog has the change but the owner's not  - click pull request -- new pull request (green buttom)
	• Automatic comparison of traces
	• Create pull request (send the commit message to the owner)
