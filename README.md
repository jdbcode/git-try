# git-try
A place to try git functions without messing up good repos



#### Working with git-RStudio-GitHub

*Good reference*: [Hadley's documentation](http://r-pkgs.had.co.nz/git.html])

##### Author attribution
When using the RStudio git interface make sure to add user and email to the repository's config file

.git/config file

<pre>[user]
	name = jdbcode
	email = jstnbraaten@gmail.com</pre>
	
##### Local branch creation and master merge in RStudio with shell
*branch is not backed up on github*

1. open the shell
2. create branch: `git checkout -b [branch-name]`
3. edit files, make commits (to new branch)
4. merge with master
  * checkout the master: `git checkout master`
  * merge the new branch to master: `git merge [branch-name]`
5. push to remote master

##### Create branch on github and push to it in RStudio
1. on github create a new branch
2. in RStudio pull the main branch
3. create a local branch of the same new github branch name: `git checkout -b [branch-name]`
4. edit files, make commits (to new branch)
5. initialize push to remote branch from shell: `git push -u origin [branch-name]`
6. now RStudio git GUI should work for pushing to remote branch

*alternatively get tracking going right way after creating the branch in shell (step 3 above) using this: `git push --set-upstream origin [branch-name]`. This way you don't need to do your first push with the -u flag in line 5 above*
