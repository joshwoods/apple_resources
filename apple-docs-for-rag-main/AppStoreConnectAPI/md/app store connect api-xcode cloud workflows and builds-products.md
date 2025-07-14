

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Products 

API Collection

# Products

Read information about the products Xcode Cloud detected or delete a product and all its associated information.

## Overview

The `ciProducts` resource represents the products Xcode Cloud detected when you started using Xcode Cloud. The resource includes information associated with the product like your app, workflows, builds, and Git repositories.

In addition to viewing your product and its associated information, you can use the `ciProducts` resource to delete a product and its associated data.

Important

Deleting a product deletes all associated data, including build information like build artifacts, and can’t be undone.

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Xcode Cloud Products

List All Xcode Cloud Products

Get a list of all products you created in Xcode Cloud.

Read Xcode Cloud Product Information

Get information about a specific Xcode Cloud product.

List All Additional Repositories for an Xcode Cloud Product

List all additional Git repositories you associated with an Xcode Cloud product.

Read App Information for an Xcode Cloud Product

Get the app in App Store Connect that’s related to an Xcode Cloud product.

List All Xcode Cloud Builds for an Xcode Cloud Product

List all builds Xcode Cloud performed for a specific product.

List All Primary Git Repositories for an Xcode Cloud Product

List all primary Git repositories for a specific Xcode Cloud product.

List All Workflows for an Xcode Cloud Product

List all workflows for a specific Xcode Cloud product.

Read the Xcode Cloud Product for an App

Get the Xcode Cloud product information for an app you build with Xcode Cloud.

### Deleting Xcode Cloud Products

Delete a Product

Delete an Xcode Cloud product and all of its associated workflows, builds, and artifacts.

### Objects

object CiProduct

The data structure that represents a Products resource.

object CiProductResponse

A response that contains a single Products resource.

object CiProductsResponse

A response that contains a list of Products resources.

## See Also

### Xcode Cloud Products and Workflows

Workflows

Manage Xcode Cloud workflows and view workflow details like actions and start conditions.

macOS Versions

Read macOS version information you configure for an Xcode Cloud workflow.

Xcode Versions

Read Xcode version information you configure for an Xcode Cloud workflow.

