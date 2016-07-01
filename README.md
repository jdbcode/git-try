# git-try
A place to try git functions without messing up good repos


### Reminders
When using the RStudio git interface make sure to add user and email to the repository's config file

.git/config file

<pre>[user]
	name = jdbcode
	email = jstnbraaten@gmail.com</pre>
	
##### working on branch in R
1. open the shell
2. create branch: `git checkout -b [branch name]`
3. edit files, make commits (to new branch)
4. merge with master
  * checkout the master: `git checkout master`
  * merge the new branch to master: `git merge [branch name]`
5. push to remote master
