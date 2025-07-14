

- Xcode
- Source control management
-  Combining code changes in a source control repository 

Article

# Combining code changes in a source control repository

Integrate code changes from multiple sources and resolve conflicts between different versions of code using source control tools in Xcode.

## Overview

If you use source control to work on code with collaborators or to manage multiple versions of your Xcode project for different releases, eventually, you need to sync code changes between versions. Git source control provides a mechanism for combining sets of code changes by merging those changes together, and Xcode provides a visual interface for performing a *merge*.

### Merge code changes

After you complete work in a feature or bug fix branch, you merge your changes into your main development or production branch. Alternatively, you merge other updates from your main development or production branch into your feature or bug fix branch to resolve conflicts or to sync your work with the latest updates and ensure everything functions appropriately before merging back into your main development or production branch.

1.  Open the Source Control navigator.

2.  In the Repositories navigator, expand your repository and the Branches folder.

3.  Select the branch you want to merge into, and then Control-click and choose Switch to make that branch the current branch.

4.  Select the branch you want to merge from, and then Control-click and choose “Merge \[*from branch*\] into \[*to branch*\]”.

If there are no conflicts, Xcode completes the merge.

### Resolve conflicts with other code

In a source control repository, a *conflict* occurs when two commits have incompatible changes and Git can’t merge the changes automatically. For example, a conflict might occur when two developers change the same lines in the same source file.

When you attempt to merge changes in Xcode, if there are conflicts, Xcode presents a comparison view for you to review and resolve the conflicts.

To resolve a conflict, click the numbered change for that conflict and select which option you want to use to resolve it:

- Choose Left

- Choose Right

- Choose Left Then Right

- Choose Right Then Left

After you choose a resolution for each conflict, Xcode enables the Merge button. Click the Merge button to complete the merge, or click Cancel to abort the merge and restore your branch so you can make more changes before merging.

## See Also

### Git

Organizing your code changes with source control

Streamline your collaboration workflow by managing your Xcode project’s features and releases with Git branches and tags.

Configuring source control preferences in Xcode

Customize the default Xcode Settings for connecting to Git repositories, applying code changes, and more options for configuring source control.

