
![[Git Merge2.png]]

## Git Merge
Pulls the latest features of main into the feature branch, merging the two branches, like tying a knot. 
Complete picture of the commit history and branch evolution, however can become messy.
## Git Rebase
Changes the **Base** of the feature branch to the latest release of Main, clean straightforward commit history. 
Tidies up history by moving commits to the main branch tip.

## Squash Commit
Squashing all the feature branch commits into a single commit, merged into main, like rebasing but with a single commit, you lose the fine details in the **main branch**. The feature branch still exists and still has the history. A bit of a hybrid approach. 
Consolidates commits into one, providing a clean linear history in the main branch but at the cost of detailed commit history. 

## Pros and Cons
![[Pros Cons Git Workflow.png]]