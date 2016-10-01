Here we are beginning to create our Google webpage. First I will be pushing this text file into my Git repository that I have set up. 

To push the file into my repository, first I have to add my file.

		git add "example-file.txt"

The purpose of this is to add file to staging area. Essentially, this is to "save" changes.

To see the status of the file use:
	
		git status

After adding our example file, "README.md", you will see this using git status:

		Initial commit

		Changes to be committed:
  		(use "git rm --cached <file>..." to unstage)

		new file:   README.md (highlighted green)

The files that have been added ("README.md") will appear as green highlighted text.

Finally, to commit the changes, you will use the following command

		git commit -m "These are the files being committed"

You do not need to select the files being committed because they will already be in the staging area from the git add step. The purpose of -m "example text"
is to provide a message for the commit that you will be able to see when you look at the git log. 

Here is an example of the git log once we commit the file "README.md"

		Author: Jordan Shoemaker <jrdn_shoemaker@yahoo.com>
		Date:   Sat Oct 1 13:08:14 2016 -0700

    	Committing the README.md file

The last line is the example text we provided in git commit -m "example text"

Now, looking at the git staus we see....

			On branch master
			Your branch is based on 'origin/master', but the upstream is gone.
  			(use "git branch --unset-upstream" to fixup)
			nothing to commit, working directory clean

From the last line, we see there is nothing to commit. The README.md file has been commited. 

			Now I am going to alter the README.md file, and save it. I will have to add and commit this README.md file again 

Using git log again, I can see that I have made two different commits with their messages included.

			commit 152d2bb73a0384c191c9d43c1676ad8a26e76c66
Author: Jordan Shoemaker <jrdn_shoemaker@yahoo.com>
Date:   Sat Oct 1 13:13:04 2016 -0700

    		Commiting updated README.md file explaing how the git (status, log, add, commit) work

commit a6a2909a92988138f84dd76f09725a4fe94c13b6
Author: Jordan Shoemaker <jrdn_shoemaker@yahoo.com>
Date:   Sat Oct 1 13:08:14 2016 -0700

    		Committing the README.md file


Finally, I am going to push my remote repository to the git origin master, using this command

			git push origin master


This will push all my changes to the origin master
			




