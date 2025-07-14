

- Xcode
- Xcode Cloud
-  Source code management setup 

# Source code management setup

Allow Xcode Cloud to access your Git repository.

## Overview

With Xcode Cloud, you can adopt a CI/CD practice that helps you develop and maintain your apps and frameworks. For Xcode Cloud to automatically build and test your code when you make changes, provide a continuous secure HTTPS connection on port 443 to the Git repository that contains your code.

When you configure your workspace or project to use Xcode Cloud, Xcode analyzes it to detect the Source Code Management (SCM) provider you use. On the “Grant Access to Your Source Code” sheet, click Grant Access and let Xcode guide you through your SCM provider’s native authorization flow.

Make sure you have the required permission or role to grant Xcode Cloud access to your Git repository. Additionally, if you use a self-hosted SCM provider — for example, Bitbucket Server — make sure Xcode Cloud can access your Git repository. For information on required permissions, roles, and IP address ranges that Xcode Cloud uses, see Use a remote source control repository.

Note

Xcode Cloud comes with support for Git LFS.

## Topics

### Bitbucket Cloud and Bitbucket Server

Connecting Xcode Cloud to Bitbucket Cloud

Allow Xcode Cloud to access your Bitbucket Cloud repository.

Connecting Xcode Cloud to Bitbucket Server

Allow Xcode Cloud to access your Bitbucket Server repository.

### GitHub and GitHub Enterprise

Connecting Xcode Cloud to GitHub

Allow Xcode Cloud to access your GitHub repository.

Connecting Xcode Cloud to GitHub Enterprise

Allow Xcode Cloud to access your GitHub Enterprise repository.

### GitLab

Connecting Xcode Cloud to GitLab

Allow Xcode Cloud to access your GitLab repository.

Connecting Xcode Cloud to a self-managed GitLab instance

Allow Xcode Cloud to access your self-managed GitLab repository.

## See Also

### Source code management

Configuring requirements for merging a pull request

Protect stable branches by requiring a successful Xcode Cloud build or action before it’s possible to merge a pull request.

