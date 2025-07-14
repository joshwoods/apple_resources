

- Xcode
- Xcode Cloud
-  Building Swift packages and Swift Playgrounds app projects with Xcode Cloud 

Article

# Building Swift packages and Swift Playgrounds app projects with Xcode Cloud

Add your Swift package or Swift Playgrounds app project to an Xcode project to build it in Xcode Cloud.

## Overview

Xcode Cloud comes with support for the Swift Package Manager, and using Swift package dependencies in your app project requires little to no configuration. However, Xcode Cloud can’t build standalone Swift packages. To build your Swift package with Xcode Cloud:

1.  Create an app project or workspace in Xcode.

2.  Add your Swift package as a local package as described in Organizing your code with local packages.

3.  Commit your `Package.resolved` file.

4.  Create your first workflow as described in Configuring your first Xcode Cloud workflow.

When Xcode Cloud starts a build, it builds your Swift package as part of the app project.

Similarly, Xcode Cloud can’t build standalone apps you create with Swift Playgrounds. To build an app you created with Swift Playgrounds, save the Swift Playground app project to your Mac, add it to an Xcode project as described above, then configure your first workflow for the Xcode project.

Note

To learn more about building projects with Xcode Cloud that require Swift package dependencies, see Use Swift package dependencies and Git submodules.

## See Also

### Setup and maintenance

Making dependencies available to Xcode Cloud

Review dependencies and make them available to Xcode Cloud before you configure your project to use Xcode Cloud.

Configuring Xcode Cloud for your team

Start using continuous integration and delivery with Xcode Cloud as a team.

Sharing macOS and Xcode versions across Xcode Cloud workflows

Use custom aliases to share configurations with multiple workflows.

Sharing environment variables across Xcode Cloud workflows

Apply common configurations to multiple workflows by using shared environment variables.

Setting the next build number for Xcode Cloud builds

Start numbering builds from a custom build number for your existing Mac app to avoid version collisions.

Including notes for testers with a beta release of your app

Add text files to your Xcode project to provide notes to beta testers about what to test.

Removing your project from Xcode Cloud

Remove your project from Xcode Cloud to delete app and workflow data, disconnect your Git repository, and remove the Slack integration.

