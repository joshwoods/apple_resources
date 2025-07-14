

- Xcode
- Source control management
-  Configuring your Xcode project to use source control 

Article

# Configuring your Xcode project to use source control

Sync code changes between team members and development computers by setting up your Xcode project to use Git source control.

## Overview

When you’re building a project with a team, or by yourself using more than one development computer, use Xcode’s support for Git source control to coordinate code changes between team members or computers, and keep them all in sync.

Git relies on a *source control repository* to track a history of your project’s code changes and to sync those changes across other devices. Set up your Xcode project to use Git by creating and configuring a new source control repository, or by downloading an existing source control repository.

### Customize your author name and email

Before you configure a source control repository for a specific project, customize your name and email address for source control for all projects in Xcode. When you make changes to your source code and commit them to your source control repository, Xcode includes your name and email address as the author in the source control history. Users can Control-click a history entry to email the author.

To customize your name and email address for source control for all projects, choose Xcode \> Settings \> Source Control and click the Git tab. Enter your preferred author name and email address in the applicable fields.

Tip

If the Git tab doesn’t appear, make sure you select the Enable Source Control option in the General tab.

### Create a local repository with your new project

When you create a new Xcode project, one of the final steps is to specify where you want to save your project files. At this point, you can quickly create a local Git source control repository for your project by selecting the “Create Git repository on my Mac” option and then clicking the Create button.

Xcode creates your project in the folder you specify, initializes a local Git source control repository for your project, and commits all the files that it creates for your project in an initial commit. For more information, see Creating an Xcode project for an app.

### Get a project from a remote repository

You can also create a local copy, or *clone*, of an existing remote Git repository to update and sync changes with. If the repository you want to clone uses Bitbucket, GitHub, or GitLab as its host, and requires authentication, you need to set up account information to access the repository. Choose Xcode \> Settings \> Accounts, click the Add button (+), select the type of account to add, and click Continue.

In the dialog that appears, click the “Create a Token on \[*Source Control Platform*\]” button if you don’t have a token already. Otherwise, provide your account information and personal token to connect to the remote repository, and click Sign In.

To copy a remote repository, select Source Control \> Clone.

If you add one or more source control accounts, Xcode shows a list of the projects that you can select to clone. Alternatively, get a URL for a remote repository, paste it into the repository URL field, and press Enter. If the remote repository corresponds to an Xcode project, Xcode scans the project and provides a list of branches available to clone. Select a branch to clone, and provide a location for Xcode to save the cloned project.

Xcode creates a copy of the project from the remote repository, saves it in the location you specify, checks out the branch you select, and opens the project.

### Connect to a remote repository to sync changes

Share your changes with other developers on your team, or maintain a backup of your project by syncing changes with a remote repository. To sync with a remote repository, you need to configure your source control settings for your project to point to the remote repository. If you cloned your local repository from a remote repository, your project already has a connection to the remote repository. Otherwise, create a new remote repository or connect to an existing one. To accomplish these tasks, select the Source Control navigator (the second navigator from the left, next to the Project navigator). In the Source Control navigator, select the Repositories navigator.

Create a new remote repository in the Source Control navigator by Control-clicking the Remotes folder for your project and choosing New “\[*project name*\]” Remote. Provide the information and click Create to create and connect the new remote repository.

Add a connection to an existing remote repository in the Source Control navigator by Control-clicking the Remotes folder for your project and choosing Add Existing Remote. Provide a name and URL for the remote repository, and click Add to set up the connection.

### Retrieve changes from a remote repository

Get changes from the remote repository by choosing Source Control \> Pull. In the dialog that appears, select the branch with the changes you want to apply to your local repository, select the “Rebase local changes onto upstream changes” option if you want, and click Pull.

Alternatively, choose Source Control \> Fetch Changes to download the changes from your remote repository without applying them to your working copy.

### Share changes to a remote repository

When you’re ready to share your work, choose Source Control \> Push. In the dialog that appears, select the branch you want to share, select the Include Tags option if you want to push tags to the remote repository, and then click Push to sync your changes with the remote repository.

To add a collaborator to your remote repository, sign in to your source control account in a web browser and add a new collaborator in your repository’s Settings.

For information about configuring additional settings for source control management in Xcode, see Configuring source control preferences in Xcode.

## See Also

### Essentials

Tracking code changes in a source control repository

Create a history of incremental code changes to your Xcode project’s source control repository with Git commits.

