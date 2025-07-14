

- Xcode
- Source control management
-  Organizing your code changes with source control 

Article

# Organizing your code changes with source control

Streamline your collaboration workflow by managing your Xcode project’s features and releases with Git branches and tags.

## Overview

Most Xcode projects need to keep track of multiple feature and release timelines simultaneously. Git provides support for organizing different versions of code into branches and annotating your project’s significant milestones with tags.

### Organize new feature or bug fix changes in a branch

When you update source code to add a new feature or to fix a bug, keep all the changes together in a branch so that you can work with them as a unit. For example, if you decide not to add a new feature after building it without using source control, it can be a significant effort to undo the work. If you organize your work in a branch, you can decide not to merge the branch and avoid having to undo work.

Before you begin new work, choose a starting point for your branch. In Xcode, open the Source Control navigator and expand the folder with your project name. Expand the Branches folder to see a list of the current local branches, or the Remotes folder to see a list of remote repositories and branches. By default, Xcode creates a branch named *main* when you create a new project with a Git repository. Control-click the branch you want to use as your starting point, choose “Branch from \[*branch name*\]”, and then enter a name for your branch that identifies the work you’re doing. When you click Create, Xcode creates the branch and makes it current, so any changes you make and commit are part of that branch.

Make, test, and commit your changes. When your new feature or bug fix is complete and you’re ready to include your work in the main code branch, review and merge it. For more information, see Combining code changes in a source control repository.

Tip

Create a new branch from the current branch with uncommitted changes, and your changes become part of the new branch. You can’t switch to another branch if you have uncommitted changes, so commit your changes or stash them before switching to another branch.

### Set aside work in progress to make other changes

When you have work in progress that you aren’t ready to commit and you need to switch to another branch, stash your changes to save them without committing them to the repository. Choose Source Control \> Stash Changes, and optionally enter a description of your changes.

Xcode creates a stash entry with your changes and removes those changes from the current working environment so that you can switch branches or start working on other changes.

In the Source Control navigator, view the Stashed Changes folder under your project folder. Select a stashed change item to review the changes in the comparison view. To add the changes to your current work, Control-click the stashed change item and choose Apply Stashed Changes. Xcode updates the current working environment with the stashed changes so you can continue making updates or commit your changes to the repository.

When you no longer need the stashed changes, Control-click the stashed change item and choose Delete to remove it.

### Mark releases and significant milestones

Add tags to commits that represent a significant milestone, like a release or large feature addition, to make them easy to find in source control history.

In the Source Control navigator, expand the folder with your project name. Expand the Branches folder to see a list of the current local branches, select a branch, and then optionally select a commit in the history list. Control-click either the branch or the commit, and choose Tag.

If you select the branch, Xcode applies the tag to the most recent commit in the branch. Enter a short string for the tag, and, optionally, a more detailed message. Click Create, and Xcode creates the tag and marks the commit with it.

In the Source Control navigator, under the folder with your project name, expand the Tags folder to see and navigate to tagged commits.

## See Also

### Git

Combining code changes in a source control repository

Integrate code changes from multiple sources and resolve conflicts between different versions of code using source control tools in Xcode.

Configuring source control preferences in Xcode

Customize the default Xcode Settings for connecting to Git repositories, applying code changes, and more options for configuring source control.

