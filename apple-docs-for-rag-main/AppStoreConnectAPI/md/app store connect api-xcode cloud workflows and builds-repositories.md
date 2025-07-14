

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Repositories 

API Collection

# Repositories

Read detailed information for each repository Xcode Cloud can access, including Git references and pull requests.

## Overview

The `scmRepositories` resource represents Git repositories Xcode Cloud can access. Use it to retrieve all repositories for a source code management provider you connected to Xcode Cloud and read:

- The name and owner of the repository

- The date when Xcode Cloud last accessed the repository

- The HTTP and SSH URLs for cloning the repository

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Repository Information

List All Git Repositories

List all Git repositories Xcode Cloud can access.

Read Git Repository Information

Get information about a Git repository that Xcode Cloud can access.

List All Git References for a Repository

List all Git references for a specific repository that Xcode Cloud can access.

List All Pull Requests for a Repository

List all pull requests for a specific repository that Xcode Cloud can access.

### Objects

object ScmRepository

The data structure that represents a Repositories resource.

object ScmRepositoryResponse

A response that contains a single Repositories resource.

object ScmRepositoriesResponse

A response that contains a list of Repositories resources.

## See Also

### Source Code Management

Providers

Read information about source code management providers you connected to Xcode Cloud.

Pull Requests

Read pull request information such as source and destination branches.

Git References

Read information about the canonical reference for a Git branch or tag.

