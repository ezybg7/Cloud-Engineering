Version control, keeping track of changes 
[Git docs](https://git-scm.com/docs)

bash
```bash
git init
```

Initializes a repository and allows you to start version controlling your project.
Marks directory as a git project, allowing version control for tracking changes to files.
Basically, cd into what directory you want and then `git init` to create git version control by initializing a new Git repository in that directory.

When ran
1. Creates `.git` directory : Hidden folder called `.get` gets created in the root of the project.
   It contains all of Git's internal files and configurations, like : 
   - Commit history
   - Staging area (temp location that keeps changes that are "staged")
   - Local branches and references
   - Configuration files (`config`)
2. New repository state: The project is put in an un-versioned state. No files are yet tracked or committed. 
3. Starting point for version control: You can now:
   - Use `git add` to include/stage files
   - Use `git commit` to record changes / create a snapshot of their current state
   - Use other Git commands, i.e. (`git status`, `git log`)

**head**
: *the most recent changes*

bash
```bash
#Create branch
git branch branchName

#Move into the branch to make changes
git checkout branchName
```

Work on anything in that branch without affecting any files in the master branch. Commits made in the branch are alternate from the master, with its own version history.

When you're ready to merge

bash
```bash
#Checkout your master branch
git checkout masterBranch

#Merge your branch with the master branch
git merge branchName
```

The tip of your feature branch now becomes head of the master branch.
Basically they are merged and now considered one.

