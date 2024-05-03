# demogit

Certainly! Learning Git through project-based scenarios is an excellent approach. Here are some tasks you can work on to enhance your Git skills:

1. **Set Up a Git Repository**: Completed
   - Create a new directory for your project.
   - Initialize a Git repository in that directory using `git init`.

2. **Create and Switch Branches**: Completed
   - Create a new branch named "development" using `git branch`.
   - Switch to the "development" branch using `git checkout`.

3. **Add and Commit Changes**: Completed
   - Create a new file (e.g., index.html) in your project directory.
   - Add this file to the staging area using `git add`.
   - Commit the changes to the "development" branch using `git commit`.

4. **Merge Branches**:
   - Create another branch named "feature-login" from the "development" branch.
   - Make changes to the index.html file to include a login form.
   - Add and commit these changes to the "feature-login" branch.
   - Switch back to the "development" branch.
   - Merge the "feature-login" branch into the "development" branch using `git merge`.

5. **Resolve Merge Conflicts**: completed
   - Introduce a conflicting change in both the "development" and "feature-login" branches (e.g., modify the same line in index.html differently).
   - Attempt to merge the "feature-login" branch into the "development" branch.
   - Resolve the merge conflict by editing the conflicted file, then add and commit the resolved changes.

6. **View Commit History and Diffs**: completed
   - Use `git log` to view the commit history.
   - Use `git diff` to view the differences between commits or branches.

7. **Create and Apply Tags**: completed
   - Create a lightweight tag for a specific commit using `git tag`.
   - Push the tags to the remote repository using `git push --tags`.
   - Checkout a specific tag to view the project at that state.

8. **Collaborate with Remote Repositories**:completed
   - Set up a remote repository on a platform like GitHub or GitLab.
   - Add the remote repository URL to your local repository using `git remote add`.
   - Push your local branches to the remote repository using `git push`.
   - Pull changes from the remote repository using `git pull`.
   
   **Git Stash:** completed
    - Use `git stash` to temporarily store changes in your working directory without committing them.
    - Apply stashed changes to a different branch or onto the current branch.
	
	**Git Revert and Reset:**
    - Practice using `git revert` to undo a specific commit while preserving history.
    - Experiment with `git reset` to reset the current branch to a previous state, either soft, mixed, or hard.


9. **Branching Strategies**: completed
   - Explore different branching strategies like GitFlow or GitHub Flow.
   - Implement a branching strategy of your choice for your project.

10. **Additional Tasks**:
   - Experiment with Git rebase to rewrite commit history.
   - Use Git cherry-pick to apply specific commits to another branch.
   - Practice Git reset to undo changes or move HEAD to a previous state.


12. **Rebase and Squash Commits:**
    - Experiment with rebasing your feature branches onto the latest changes in the "development" branch.
    - Squash multiple commits into a single commit using interactive rebase (`git rebase -i`).

13. **Cherry-pick Commits:**
    - Create a new branch and cherry-pick specific commits from other branches onto it.
    - Explore how cherry-picking can be useful in integrating specific changes into different branches.

14. **Git Hooks:**
    - Set up a pre-commit hook to enforce code formatting rules (e.g., using tools like ESLint or Prettier).
    - Implement a post-receive hook on the remote repository to trigger deployment scripts after a successful push.

15. **Managing Large Files:**
    - Investigate Git LFS (Large File Storage) and configure it to handle large binary files in your project.
    - Experiment with Git's built-in mechanisms for handling large files, such as `git annex` or `git filter-repo`.

16. **Git Submodules or Subtrees:**
    - Learn about Git submodules or subtrees and how they can be used to manage dependencies in your project.
    - Integrate a submodule or subtree into your project and explore how to update it.

17. **Git Workflows with CI/CD:**
    - Integrate your Git repository with a CI/CD tool like Jenkins, Travis CI, or GitHub Actions.
    - Set up automated testing and deployment pipelines triggered by Git events such as pushes or pull requests.

18. **Git GUI Tools:**
    - Experiment with Git GUI tools such as Sourcetree, GitKraken, or GitHub Desktop.
    - Compare the features and workflows of these tools with the command-line interface.

19. **Git Aliases:**
    - Create custom Git aliases to streamline common commands or sequences of commands.
    - Share your favorite aliases with your team and encourage their adoption.

20. **Documentation and Collaboration:**
    - Use Git-based documentation tools like Markdown or AsciiDoc to write project documentation.
    - Collaborate with your team members on documentation updates using Git's version control capabilities.



21.

22. 

23. **Git Bisect:**
    - Simulate a bug in your project and use `git bisect` to perform a binary search through commit history to identify the first commit that introduces the bug.

24. **Git Submodules or Subtrees (Advanced):**
    - Explore advanced usage of Git submodules or subtrees, such as updating submodules to specific revisions or working with nested submodules.
    - Investigate the differences between submodules and subtrees and choose the appropriate approach for your project.

25. **Git Merge Strategies:**
    - Experiment with different merge strategies such as recursive, octopus, or theirs, and understand their advantages and limitations.
    - Compare the results of merging using different strategies in various scenarios.

26. **Git Hooks (Advanced):**
    - Implement custom Git hooks tailored to your project's specific requirements, such as pre-push hooks for enforcing code review policies or post-merge hooks for triggering deployment tasks.

27. **Git Internals:**
    - Dive into the internal workings of Git by exploring its object model, index, and repository storage structure.
    - Gain insights into how Git stores and manages commits, branches, and tags.

28. **Git Branching Visualization:**
    - Use tools like Gitk, Gitg, or third-party visualization tools to visualize your project's branching history and commit graph.
    - Analyze branching patterns and commit flows to identify areas for optimization or improvement.

29. **Git Anomaly Detection:**
    - Develop scripts or tools to detect anomalies or irregularities in your Git repository, such as large commits, frequent reverts, or divergent branches.
    - Implement automated checks to maintain repository hygiene and consistency.

30. **Git Best Practices Review:**
    - Conduct a comprehensive review of your project's Git usage against industry best practices and standards.
    - Identify areas for improvement in branching strategies, commit hygiene, documentation practices, and collaboration workflows.


-------------------------------------------------------------------------------------------------------
Practicing

1..**Set Up a Git Repository**: Completed

Created portfolio folder , inside intialized git init

tried to create new branch from the master getting this error
Error -> fatal: Not a valid object name: 'master'.

solution
A non-bare git init will also create the same files, in a hidden .git directory in the root of your project.


2 ..**Create and Switch Branches**: Completed

To create a new branch without committing on master, you can use: git checkout -b <branchname>

$ git checkout -b feature/development
Switched to a new branch 'feature/development'
git branch --all or git branch , u cant see anyone 
git branch only shows branches with commits. Try git status to see the current branch name even if it has no commits.

other solution
First, you have to use git add . or git add <file-name> , then you have to use git commit -m "committed successfully"
now you can create a new branch

3. **Add and Commit Changes**: Completed

I created demo index.html with touch command and added to staged area 
when I clicked on $ git add .
I gave this output
warning: in the working copy of 'assets/css/styles.css', LF will be replaced by CRLF the next time Git touches it

Solution
CR and LF are a special set of characters that help us format our code.

CR (\r) stands for CARRIAGE RETURN. It puts the cursor at the beginning of a line, but it doesn't create a new line. This is how classic Mac OS works (not applicable today unless you are dealing with old files).

LF (\n) stands for LINE FEED. It creates a new line, but it doesn't put the cursor at the beginning of that line. The cursor stays back at the end of the last line. This is how Unix (including macOS) and Linux work.

CRLF (\r\n) creates a new line as well as puts the cursor at the beginning of the new line. This is how we see it in Windows OS.

Git uses LF by default. So when we use Git on Windows it throws a warning like "CRLF will be replaced by LF" and automatically converts all CRLF into LF, so that code becomes compatible.


4. **Merge Branches**:

to get the tree view 
git log --oneline --decorate --graph --all

Tree with date and author
$ git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --all

To accept their changes: git merge --strategy-option theirs
To accept your changes: git merge --strategy-option ours

merge conflicts issues
git mergetool reference
https://gist.github.com/karenyyng/f19ff75c60f18b4b8149

when I used to merge from feature/login to feature/development I created merge conflicst , if it has conflict also it was merging
giving
$ git merge feature/development
Updating 3c19a45..1d2bbd0
Fast-forward
 demoIndex.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)


what is fast farawrd then
$ git merge --no-ff feature/login
Merge made by the 'ort' strategy.
 conflict.txt | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)


need to learn Merge made by the 'ort' strategy.


After I perform a Git merge and resolve the conflicts, there are leftover .orig versions of the conflicting files. How can I automatically delete those after the conflict is successfully resolved?

 git config --global mergetool.keepBackup false
 
 drop down of read me file
 https://gist.github.com/apaskulin/1ad686e42c7165cb9c22f9fe1e389558
 
 
 **View Commit History and Diffs**:
 
 not able to come out f git logs
 By pressing the q key on the keyboard, we can exit the git log without duplicating the commit default history.
 
 press q
 
 cn commiter name
 h commid id
 cd commit date
 $ git log --oneline --graph --pretty=format:"%cn commited  %h on %cd"
 
 https://www.atlassian.com/git/tutorials/git-log

git Diffs
https://www.freecodecamp.org/news/git-diff-command/
git diff HEAD <file_name>
git diff <file_name>
git diff --staged <file_name> or  git diff --cached <file_name>,
git diff <branch_name1> <branch_name2> <file_name>
git diff <commit_hash> <commit_hash> <file_name>

A – Old version of file
B – New version of file


**Create and Apply Tags**:

https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-tag


**Collaborate with Remote Repositories**:

Below will reinitialize your local repo; also clearing remote repos (ie origin):

git init
Then below, will create 'origin' if it doesn't exist:

git remote add origin [repo-url]
Else, you can use the set-url subcommand to edit an existing remote:

git remote set-url origin [repo-url]
Also, you can check existing remotes with

git remote -v

Now I have 2 brnaches 
feature/development
feature/login

I need to push these branch to my remote not a master branch

Push All Branches to GitHub:
First, make sure you've added the GitHub repository as a remote to your local repository (you can use the git remote add command as mentioned in the previous response if you haven't done so already).
Then, push all branches to GitHub using the --all flag:

-u option is the short version of --set-upstream - they are the same.
git push --set-upstream origin new-branch
Once you create a new branch, you must run the –set-upstream switch the first time you perform a push.

This use of the –set-upstream parameter (two dashes) only needs to happen once. All subsequent git push commands automatically move local branch changes up to the remote branch.


**Branching Strategies**:
https://nvie.com/posts/a-successful-git-branching-model/

Git Stash
https://www.atlassian.com/git/tutorials/saving-changes/git-stash
https://www.freecodecamp.org/news/git-stash-commands/
The git stash command takes your uncommitted changes (both staged and unstaged), saves them away for later use, and then reverts them from your working copy. 


git blame
The git blame command is used to examine the contents of a file line by line and see when each line was last modified and who the author of the modifications was. The output format of git blame can be altered with various command line options. Online Git hosting solutions like Bitbucket offer blame views, which offer a superior user experience to command line git blame usage. git blame and git log can be used in combination to help discover the history of a file's contents. The git log command has some similar blame functionality, to learn more visit the git log overview page.

git clean coomand 
https://www.atlassian.com/git/tutorials/undoing-changes/git-clean

git clean -n for which are the files to now remove

git clean -f removed all untacked file

git clean -di  it will go to interactive mode


**Git Revert:**

https://www.atlassian.com/git/tutorials/undoing-changes/git-revert

git reset
https://www.cloudbees.com/blog/git-reset-undo-changes

first commit for restfile1.txt id 
commit c1e1c36e9ab549d0461b645ebf9f84c4dbf86682


git hard remove the commit history and nothing will be in git head moved to prevous 

git mixed means staging file will comes to working directory head stayes in same postition

git soft 



