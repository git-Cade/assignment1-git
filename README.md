
# assignment1-git
**CS 390 - Objects and Design - Spring 2021**

Cade Lilley  
Pacific Lutheran University  
lilleycr@plu.edu
CS 390  - Dr. Wolff

## Walk Through

1. **Step One**
	1. `touch Hello.java` - Edited added class Hello with main method with print line of Hello, World
	2. Updated README.md
	3. `touch .gitignore`
	4.  `git status` - Gets current local server status. Shows additions, changes, and deletions
	5. `git add .` - Adds all new files/changes
	6. `git status`
	7. `git commit -m "..."` - Create commit with message
	8. `git push` - Push to origin/main
2. **Step Two**
	1. Created `newfile1.txt` and `newfile2.txt`
	2. `git add .` to add new files
	3. `git status` to verify new files are added
	4. `git commit -m "..."` created commit with new files and message
	5. Repeated after deleting `newfile2.txt` and adding `replacement.txt`
3. **Step Three**
	1.  Created new directory and did a git clone. (Now referred to as project B)
	2. After editing a file
		1. `git status`
		2. `git add .`
		3. `git commit -m "..."`
		4. `git push`
	3. Repeated step 2 in project B directory, failed to push due to conflict
	4. Used a simple `git pull` in order to get the updated files from github server.
	5. Used `git push` to push changes. Now able to after synchronizing with github server.
4. **Step Four**
	1. Made changes to Hello.java in project A directory. Used the following commands to commit and push:
		1. `git status`
		2. `git add Hello.java`
		3. `git commit -m "..."`
		4. `git push`
	2. Made changes to Hello.java in project B directory. Did not commit the changes.
	3. Attempted fetch and merge, to no avail. Merge step failed. Used second options (stashing) in order to resolve this issue. Used information from next step (step 5) in order to solve this issue when `git stash pop` caused a merging conflict.
5. **Step Five**
	1. Since this problem asks for the problem that I created in step four, I applied the method of opening the respective conflicting file in an editor and using the line markers to select which line I wanted to keep, and which I should delete. I think staged the file, and commit it. Finally, I pushed the resolved conflict file.
		1. `git add Hello.java`
		2. `git commit -m "Fixed local conflict when attempting with pull from server. Updated file now available"`
		3. `git push`
