==================================Git Notes========================================

Checkout branch:
1.git checkout 'branch name';
2. git checkout -b 'branch name '; it will create local branch

Git Commit:
1.git commit -m 'commit message';
2. git commit -am 'file path '  // it will add our local changes to stage and the commit the changes

Time Tavel with Reset and Reflag:
i. there are threee types of Reset modes:
	--soft
	--default (mixed)
	--hard  // it will changes all your local changes with the given commit id
examples: 
git Reset 'commit_ID' --soft/hard/mixed

Commit logs:
1. git log --oneline // gives all previous commit id's only
2 git reflog   // gives all previous changes like commits, merges, checkouts ext

Git configs:
git config --global user.name 'user_Name'
git config --global user.email 'email_id'

Pushing Our local project to GitHub:
1. we need to create repository in the git with default settings.
2. there are two commands for getting the intraction with github and our local changes
i. git remote add origin 'https://github.com/sriaktnh/demo-app002.git
ii. git push -u origin master

Git branch:
1. git branch 'branch_name' // it will create new branch

Generating SSH key in git :
1. create a folder with the name '.ssh' then move to that file cd .ssh
2. generate ssh ky using below command
command: i.   ssh-keygen -t rsa -C 'email-id'   // -t means type to specify which method you are using to generate key ex: rsa and -C means combining rsa and your email id.
	ii. ssh -T git@github.com // to pss private key using git
3. copy the public key in git hub
4. connect github using (ii) this command

Cloning existing project from github:
1. git clone 'git@github.com:sriaktnh/web-application.git' // you can specify the folder name at end.

Check Remote Connection:
1. git remote -v

Mergiing the branches in local:
1. git merge 'branch name'

Push your local project to git:
1. create a new repository in git.
2. goto your project in git bash and run 'git init' it will add git feature to your local project
3. commit all your changes in locally by using below commands 
  i) git add .
  ii) git commit -m 'commit massege'
4. add remote connection to your project.
  i) copy the ssh key from the github
  ii) git remote add origin 'ssh key'
  iii) check remote key is added or not by using "git remote -v"
5. push your local changes to git.
  i) git push --set-upstream origin master
  ii) if above command gives any error create local branch "git checkout -b 'branch-name" 
  iii)push this branch to git "git push --set-upstream origin 'branch-name' "
  
  Git squash:
  1. git rebase -i HEAD~[no. of commits]
  examples git rebase -i HEAD~2
