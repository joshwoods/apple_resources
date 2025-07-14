

- Xcode
- Source control management
-  Tracking code changes in a source control repository 

Article

# Tracking code changes in a source control repository

Create a history of incremental code changes to your Xcode project’s source control repository with Git commits.

## Overview

When you use a source control repository to manage your Xcode project, you save changes to your repository in incremental states called commits. A *commit* consists of a snapshot of your project’s state at a particular point in time, a message that describes the set of changes from the previous commit, and additional metadata like a unique hash that identifies the commit.

In Xcode, you can save your project’s current state in a commit, navigate the history of your project’s previous commits, compare changes between specific commits, and quickly restore to a previous commit.

### Save your project’s current state

As you make changes to your source code in a source control repository, Xcode tracks those changes and highlights them in the Project navigator and in the source editor. While you’re working on a change, look at the Project navigator to see your changes in the current branch.

The Project navigator annotates files with changes since the last commit, using an *A* for new files or an *M* for modified files. To compare changes in one source file, open the file and click the Enable Code Review button in the upper-right corner of the Xcode window.

The comparison view highlights changes between the current source code and the most recent commit. You can choose whether to view changes inline or side by side by clicking the Adjust Editor Options button.

The comparison view allows you to:

- Navigate between the numbered changes using the arrows at the bottom of the center column.

- Click a number in the center column to select and discard a change.

- Choose other commits to compare your current changes against.

When you’re done making changes, commit them to save them permanently in your source control repository. Choose Source Control \> Commit, and review your changes.

In the Project navigator, select a file in the list to view the code changes for that file. Click the numbered selector between the left and right sides of the comparison view, and then choose Don’t Commit to exclude an individual change from your commit, or choose Discard Change to remove a change. Select checkmarks to indicate which files to include in your commit.

Warning

When you add a new file or delete an unused file, you must commit both the file and the Xcode project file (called `project.pbxproj`) together for your project to remain in a consistent state.

Document your changes with a commit message that describes what your commit accomplishes. Click the “Commit \[*number*\] files” button to commit your changes, or click Cancel to continue working without committing to the repository. Xcode shows the commit message you provide when you look at the source control history.

If you don’t want to commit any of your changes, and want to remove them, choose Source Control \> Discard All Changes, and click Discard. Xcode removes all the current changes and restores your source files to the most recent commit.

### View a history of project states

Xcode has a commit history view that lets you view historical changes for your source control repository when you’re investigating a bug or adding code for a new feature.

1.  Open the Source Control navigator.

2.  In the Repositories navigator, expand your repository and the Branches folder.

3.  Select a branch to display a list of commits.

4.  Double-click a specific commit to display the comparison view, and see additional information about the commit in the Source Control inspector.

### Compare code between specific project states

To compare code between specific commits, select the branches and commits to compare from the bottom bar in the comparison view.

### Restore your project to a previous state

You can quickly restore your code to a previous state in your source control repository by checking out a specific commit. Xcode restores your project files to the state that the commit you choose specifies.

Before you restore a previous commit of the code, make sure you don’t have any uncommitted changes. If you do, you can either discard the changes (Source Control \> Discard All Changes) or save them to apply later by stashing them (Source Control \> Stash Changes).

1.  Open the Source Control navigator.

2.  In the Repositories navigator, expand your repository and the Branches folder.

3.  Select the branch that contains the commit you want to restore.

4.  In the detail view, Control-click the desired commit and choose Switch to “\[*commit-hash*\]”.

5.  In the confirmation dialog, click Switch. Xcode restores your project’s state to the earlier commit.

To learn more about restoring stashed changes, see Organizing your code changes with source control.

## See Also

### Essentials

Configuring your Xcode project to use source control

Sync code changes between team members and development computers by setting up your Xcode project to use Git source control.

