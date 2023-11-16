GameDoc file: https://docs.google.com/document/d/1Acvv1_Qo5ULFgnNSELUJTlE4iSAgsawNBOUR5ZPp31I/edit
Common Git Commands:
	To create a new branch: 
		git branch nameOfBranchHere
	To swap to a branch: git 
		checkout nameOfBranchHere
	To add changes to the stage: 
		git add -A
	To commit changes: 
		git commit -m "brief word or phrase describing changes here"
	To push changes to GitHub: 
		git push origin nameOfBranchHere
	To pull changes and merge them with your file:
		git fetch
		git merge origin/nameOfBranchHere
		NOTE: you must do this with each branch that you want a copy of. For example, if you want a copy of my Testing branch, you need to create a Testing branch, then git fetch and git merge origin/Testing to get a copy of that branch.

	To UPDATE the branch you're working on to the latest changes:
		(Ensure you're currently on the branch you're working on, and NOT the main branch)
		git rebase origin/main
	
	REMOVAL COMMANDS
	To remove UNSTAGED changes:
		git clean -df
		git checkout -- .
	To remove STAGED changes:
		git reset HEAD -- .
	To delete a branch:
		git branch -d nameOfBranchHere