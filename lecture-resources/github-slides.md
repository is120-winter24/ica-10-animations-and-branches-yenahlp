# Slide 1
## GitHub Branches, Merging, and Pull Requests
# Slide 2
## Agenda
- Prayer
- AIS Announcements
- Lecture
- ICA
# Slide 3
## Review of what we know already
Directories (or folders, projects, workspaces, etc.) that we create and work on can either be .git repositories or not. 
- What is a .git repository?
- What is version control?
By default when a .git repository is made, it is on the master (sometimes main) branch.
- What does that mean?
# Slide 4
## The idea of branching
What if you and someone else are working on the same project and you both want to make changes to the same file? 
Branching is the way to work on different versions of a repository at one time. 
By default your repository has one branch named master which is considered to be the definitive branch.
We use branches to experiment and make edits before committing them to master.
Typically, each new task or feature is created in a branch.
You can create a new branch with the git command:
```bash
git checkout -b "branch-name"
```
# Slide 5
## The idea of branching
When you create a new branch, Git keeps track of which commit your branch "branched" from.
This means that your branch knows where it came from and can keep track of the changes that have been made to the branch.
When you create a new branch, you are creating a new "timeline" of changes that are separate from the master branch.
At any time, you can switch back to the master branch with the git command:
```bash
git checkout master
```
Or any other branch in your repository, with:
```bash
git checkout branch-name
```
You need to be sure to commit (or discard of) any changes you have made before switching branches.
# Slide 6
## So, we've made a branch, now what?
Once you have made a branch, you can start making changes to the files in your project, as normal.
Save, stage, and commit your changes as you normally would. You could even push your changes to the remote repository, if you want!
Whenever we're making changes and commits to a branch, we're doing so in isolation. We want to be sure that our changes are being made on the correct branch.
We can check the status of our branch with the git command:
```bash
git status
```
This will show us what branch we are on and what files have been changed, added, or deleted.
You can also check what branch you are on (and what branches exist) with the git command:
```bash
git branch
```
# Slide 7
## Merging branches
Once you have made changes to your branch and you are ready to merge those changes back into the master branch. We do so by creating a pull request.
A pull request is a request to merge changes from one branch into another.
When you create a pull request, you are asking the repository owner to review your changes and approve them before they are merged, as we want to be sure that the changes are correct and won't break anything.
# Slide 8
## Making a Pull Request
To make a pull request, you need to push your branch to the remote repository. Do so with the git command:
```bash
git push origin branch-name
```
Once you have pushed your branch to the remote repository, you can go to the repository on GitHub and create a pull request.
You can do this by clicking the "New pull request" button on the repository's page.
You can then select the branch you want to merge into the branch that you want to merge into, and create the pull request.
# Slide 9
## Merging a Pull Request
Once you have created a pull request, the repository owner can review your changes and approve them.
Reviewing changes involves the process of looking at the changes that have been made and making sure that they are correct and won't break anything.
Once the changes have been reviewed and approved, the repository owner can merge the pull request.
The approval process is typically done by adding comments and suggestions to the code where appropriate.
If at any point there are things that need to be changed, the repository owner can request changes to the pull request.
# Slide 10
## Merging a Pull Request
After subsequent change requests have been remediated, the repository owner can approve the pull request. Approving the pull request means that the changes have been reviewed and are ready to be merged. Merging the pull request means that the changes that have been made in the branch are now part of the branch that the request intended to merge into.
# Slide 11
## Let's practice!
