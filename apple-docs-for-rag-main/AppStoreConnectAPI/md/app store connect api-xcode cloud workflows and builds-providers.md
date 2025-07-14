

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Providers 

API Collection

# Providers

Read information about source code management providers you connected to Xcode Cloud.

## Overview

The `scmProviders` resource represents the source code management (SCM) providers you connected to Xcode Cloud. Use it to access these SCM providers and read the following information for each provider:

- A unique identifier

- The provider’s type

- The provider’s URL

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Provider Information

List All Source Code Management Providers

List all source code management providers you connected to Xcode Cloud.

Get a Source Code Management Provider

Get information about a specific source code management provider you connected to Xcode Cloud.

List all Repositories for a Source Code Management Provider

List all Git repositories for a specific source code management provider you connected to Xcode Cloud.

### Objects

object ScmProvider

The data structure that represents a Providers resource.

object ScmProviderResponse

A response that contains a single Providers resource.

object ScmProvidersResponse

A response that contains a list of Providers resources.

## See Also

### Source Code Management

Repositories

Read detailed information for each repository Xcode Cloud can access, including Git references and pull requests.

Pull Requests

Read pull request information such as source and destination branches.

Git References

Read information about the canonical reference for a Git branch or tag.

