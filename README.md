


TASKS AND ASSIGNMENTS


Basic Version Control:

Create a new public repository on GitHub (use the Initialize this repository with:Add a README file option to make sure repo was created with default README)

Clone the repository to your local machine.

Create and checkout to a new branch called develop

Make changes to the ReadMe file by adding the following write-ups

Explain version control.

Explain difference between git and github

List 3 other github alternatives

Explain the difference between git fetch and git pull,

Explain in simple terms git rebase and the command for it

Explain in simple terms git cherry-pick and the command for it

Save the changes, and commit them.

Push the branch to GitHub and create a pull request to the main branch.

Merge the pull request.






1.Explain version control.
Ans:
Version control is a system that records changes to a file or
set of files over time, allowing you to recall specific versions
of your work at any given point. It is a crucial tool in software 
development and collaborative projects, enabling multiple contributorsto work on 
the same codebase while keeping track of changes, managing conflicts, 
and ensuring the integrity of the project



2.Explain difference between git and github
Ans: Git is the version control system, while GitHub 
is a platform that hosts Git repositories and provides
 additional collaboration features. Git is used locally 
on a developer's machine, while GitHub is a centralized 
platform that facilitates collaborative development, code hosting, 
and project management. Other platforms, such as GitLab and Bitbucket, 
also serve similar purposes to GitHub.

3.List 3 other github alternatives

Ans :
 1. Bitbucket
 2. GitLab
 3. SourceForge

4.Explain the difference between git fetch and git pull.
Ans:Both git fetch and git pull are Git commands used to update your local repository 
with changes from a remote repository. However, they have different behaviors, 
and understanding their distinctions is essential.

git fetch:
Purpose:

Fetches changes from the remote repository to your local repository without merging them into your working directory.
It updates the remote-tracking branches, allowing you to see what changes exist in the remote repository.
Behavior:

Downloads new branches, updates existing ones, and retrieves new objects 
(commits, tags, etc.) without modifying your working directory or your local branches.
It does not automatically merge the changes into your local branches.


git pull:
Purpose:

Fetches changes from the remote repository and automatically merges them into your current working branch.
It is essentially a combination of git fetch and git merge.
Behavior:

Downloads changes from the remote repository and incorporates them into your local working directory and branch.
It automatically merges the changes, potentially resulting in a merge commit.
Command:









5.Explain in simple terms git rebase and the command for it.

Ans:In simple terms, git rebase is a Git command that allows you to rewrite the commit history
 of a branch. It's a way to move, combine, or modify commits to create a cleaner and more linear project history.

Here's a basic analogy:

Imagine you are building a tower of Lego blocks (commits), and each block represents a change to your project. 
Rebase is like rearranging or adjusting the position of some blocks to make the tower look neater and more organized.

Basic git rebase Command:
bash
Copy code
git rebase <base_branch>
<base_branch> is the branch you want to rebase onto.
Simple Explanation:
Starting Point:

Suppose you have a branch with some commits, and there are new
 changes in the main branch (or any base branch).
Using git rebase:

When you perform a rebase, Git takes your branch's changes and applies
 them on top of the latest changes in the base branch.
Result:Your branch's commit history is now more linear, and it appears
 as if you made your changes directly on top of the latest base branch changes.








6.Explain in simple terms git cherry-pick and the command for it 

Ans:In simple terms, git cherry-pick is a Git command that allows you to pick or copy a specific commit 
from one branch and apply it onto another branch. It's like choosing a particular change from one
 branch and bringing it into another branch.

Here's a simple analogy:

Imagine you have a recipe book (a Git repository) with different recipes (commits) on different pages (branches). 
Cherry-picking is like taking a recipe from one page and copying it to another page.

Basic git cherry-pick Command:
bash
Copy code
git cherry-pick <commit_hash>
<commit_hash> is the unique identifier (hash) of the commit you want to cherry-pick.
Simple Explanation:
Choose a Commit:

Identify the commit you want to pick from one branch. This could be a bug fix, a new feature, or any change.
Cherry-Pick to Another Branch:

Use git cherry-pick to copy that specific commit and apply it onto another branch.
Result:

The changes from the cherry-picked commit are now applied to the new branch.
Example:
bash
Copy code
# Switch to the branch where you want to apply the commit
git checkout target-branch

# Cherry-pick the specific commit from another branch
git cherry-pick abc123
In this example, abc123 is the hash of the commit you want to cherry-pick.

Important Notes:
Conflict Resolution:

Similar to git rebase, conflicts may arise during cherry-pick if the 
changes in the picked commit conflict with the changes in the target branch. Resolve conflicts manually.
Commit Hash:

Ensure you provide the correct commit hash for cherry-pick.
Usage Scenario:

Cherry-pick is often used when you want to selectively bring changes 
from one branch to another without merging the entire branch.


