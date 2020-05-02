==================================Git Notes========================================

Checkout branch:
1.git checkout 'branch name';
2. git checkout -b 'branch name '; it will create local branch

Git Commit:
1.git commit -m 'commit message';
2. git commit -am 'file path '  // it will add our local changes to stage and the commit the changes

Time Tavel with Reset and Reflag:
1.git hist   // to get the commit histery
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


