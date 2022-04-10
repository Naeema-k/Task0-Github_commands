# Task0-Github_commands
>|SETUP-
Configuring user information used across all local repositories|
1. **git config --global user.name “[firstname lastname]”**
set a name that is identifiable for credit when review version history
2. **git config --global user.email “[valid-email]”**
set an email address that will be associated with each history marker
3. **git config --global color.ui auto**
set automatic command line coloring for Git for easy reviewing
>|SETUP & INIT-
Configuring user information, initializing and cloning repositories|
4. **git init**
initialize an existing directory as a Git repository
5. **git clone [url]**
retrieve an entire repository from a hosted location via URL
>|STAGE & SNAPSHOT-
Working with snapshots and the Git staging area|
6. **git status**
show modified files in working directory, staged for your next commit
7. **git add [file]**
add a file as it looks now to your next commit (stage)
8. **git reset [file]**
unstage a file while retaining the changes in working directory
9. **git diff**
diff of what is changed but not staged
10. **git diff --staged**
diff of what is staged but not yet commited
11. **git commit -m “[descriptive message]”**
commit your staged content as a new commit snapshot
>|BRANCH & MERGE-
Isolating work in branches, changing context, and integrating changes|
12. **git branch**
list your branches. a * will appear next to the currently active branch
13. **git branch [branch-name]**
create a new branch at the current commit
14. **git checkout**
switch to another branch and check it out into your working directory
15. **git merge [branch]**
merge the specified branch’s history into the current one
16. **git log**
show all commits in the current branch’s history
>|INSPECT & COMPARE-
Examining logs, diffs and object information|
17. **git log**
show the commit history for the currently active branch
18. **git log branchB..branchA**
show the commits on branchA that are not on branchB
19. **git log --follow [file]**
show the commits that changed file, even across renames
20. **git diff branchB...branchA**
show the diff of what is in branchA that is not in branchB
21. **git show [SHA]**
show any object in Git in human-readable format
>|TRACKING PATH CHANGES-
Versioning file removes and path changes|
22. **git rm [file]**
delete the file from project and stage the removal for commit
23. **git mv [existing-path] [new-path]**
change an existing file path and stage the move
24. **git log --stat -M**
show all commit logs with indication of any paths that moved
>|IGNORING PATTERNS-
Preventing unintentional staging or commiting of files|
25. **logs/
*.notes
pattern*/**
38. Save a file with desired paterns as .gitignore with either direct string 
matches or wildcard globs
26. **git config --global core.excludesfile [file]**
system wide ignore patern for all local repositories
>|SHARE & UPDATE-
Retrieving updates from another repository and updating local repos|
27. **git remote add [alias] [url]**
add a git URL as an alias
28. **git fetch [alias]**
fetch down all the branches from that Git remote
29. **t merge [alias]/[branch]**
merge a remote branch into your current branch to bring it up to date
30. **git push [alias] [branch]**
Transmit local branch commits to the remote repository branch
31. **git pull**
fetch and merge any commits from the tracking remote branch
>|REWRITE HISTORY-
Rewriting branches, updating commits and clearing history|
32. **git rebase [branch]**
apply any commits of current branch ahead of specified one
33. **git reset --hard [commit]**
clear staging area, rewrite working tree from specified commit
>|TEMPORARY COMMITS-
Temporarily store modified, tracked files in order to change branches|
34. **git stash**
Save modified and staged changes
35. **git stash list**
list stack-order of stashed file changes
36. **git stash pop**
write working from top of stash stack
37. **git stash drop**
discard the changes from top of stash stack
