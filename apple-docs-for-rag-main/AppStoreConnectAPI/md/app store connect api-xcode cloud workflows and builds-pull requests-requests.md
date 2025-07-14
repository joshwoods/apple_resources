

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Pull Requests 

API Collection

# Pull Requests

Read pull request information such as source and destination branches.

## Overview

The `scmPullRequests` resource represents pull requests (PRs) for repositories Xcode Cloud can access. Use it to access:

- A PR’s number, URL, title, and status

- The destination and source branches

- A value that indicates whether the PR involves more than one repository

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Pull Request Information

Read Pull Request Information

Get information about a specific pull request.

### Objects

object ScmPullRequest

The data structure that represents a Pull Requests resource.

object ScmPullRequestResponse

A response that contains a single Pull Requests resource.

object ScmPullRequestsResponse

A response that contains a list of Pull Requests resources.

## See Also

### Source Code Management

Providers

Read information about source code management providers you connected to Xcode Cloud.

Repositories

Read detailed information for each repository Xcode Cloud can access, including Git references and pull requests.

Git References

Read information about the canonical reference for a Git branch or tag.

