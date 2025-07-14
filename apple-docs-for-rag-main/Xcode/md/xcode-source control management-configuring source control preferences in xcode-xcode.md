

- Xcode
- Source control management
-  Configuring source control preferences in Xcode 

Article

# Configuring source control preferences in Xcode

Customize the default Xcode Settings for connecting to Git repositories, applying code changes, and more options for configuring source control.

## Overview

Xcode lets you customize many default options for working with source control repositories. To modify the default source control preferences, choose Xcode \> Settings \> Source Control.

### Enable source control actions

In the General tab of Source Control settings, select the Enable Source Control option to enable the actions in the Source Control menu and the Source Control navigator. Enabling source control also displays the Git tab, which you use to configure Git integration options.

### Choose automatic source control behavior

After you enable source control, you can select additional options to specify which source control tasks you want Xcode to perform for you automatically.

- Refresh local status automatically: Xcode automatically refreshes the status of source control managed files when they change.

- Fetch and refresh server status automatically: For remote repositories, Xcode periodically refreshes the status of files that update on the server. (To manually refresh the status, choose Source Control \> Fetch and Refresh Status.)

- Add and remove files automatically: Xcode automatically updates working copies when adding or removing files in your projects.

- Select files to commit automatically: Xcode automatically selects which files to stage for a commit.

### Show code changes in the source editor

The Text Editing settings affect whether Xcode indicates code changes in the source editor.

- Show Source Control changes: Xcode shows the change bar, next to the lines that changed, in the gutter of the source editor.

- Include upstream changes: Xcode shows the changes committed by others (that may conflict with your edits) in the source editor gutter.

### Customize the comparison view layout

The Comparison View setting specifies where the local version of the code appears in the version editor. To show the local version on the left, choose “Local Revision on Left Side” from the pop-up menu; otherwise, choose “Local Revision on Right Side.”

### Choose sorting options for the Source Control navigator

The Source Control Navigator setting specifies how Xcode sorts the files in the Source Control navigator. To sort by name, choose “Sort by Name” from the pop-up menu; otherwise, choose “Sort by Date.”

### Customize Git settings

In the Git tab, you can configure default settings for Git repositories that you manage through Xcode.

Customize the Author Name and Author Email to use in the source control history. Users can Control-click a history entry to email the author.

Use the Ignored Files list to specify the files that you don’t want Git to commit to your source control repositories. To add an ignored file, click the Add button (+). To remove an ignored type, select an item in the list, then click the Delete button (–). To edit an item, double-click it.

Choose additional options for handling Git commands:

- Prefer to rebase when pulling: Perform a Git rebase when pulling changes instead of a merge.

- Show merge commits in per-file log: Show Git merge commits in the project history.

## See Also

### Git

Organizing your code changes with source control

Streamline your collaboration workflow by managing your Xcode project’s features and releases with Git branches and tags.

Combining code changes in a source control repository

Integrate code changes from multiple sources and resolve conflicts between different versions of code using source control tools in Xcode.

