

- App Store Connect API
-  List All Workflows for an Xcode Cloud Product 

Web Service Endpoint

# List All Workflows for an Xcode Cloud Product

List all workflows for a specific Xcode Cloud product.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciProducts/{id}/workflows
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Products resource.

## Query Parameters

`fields[ciWorkflows]`

`[string]`

Additional fields to include for each Workflows resource returned by the response.

Possible Values: `name, description, branchStartCondition, tagStartCondition, pullRequestStartCondition, scheduledStartCondition, manualBranchStartCondition, manualTagStartCondition, manualPullRequestStartCondition, actions, isEnabled, isLockedForEditing, clean, containerFilePath, lastModifiedDate, product, repository, xcodeVersion, macOsVersion, buildRuns`

`limit`

`integer`

The number of Workflows resources to return.

Maximum: `200`

`fields[ciXcodeVersions]`

`[string]`

Possible Values: `version, name, testDestinations, macOsVersions`

`fields[ciMacOsVersions]`

`[string]`

Possible Values: `version, name, xcodeVersions`

`fields[ciProducts]`

`[string]`

Possible Values: `name, createdDate, productType, app, bundleId, workflows, primaryRepositories, additionalRepositories, buildRuns`

`fields[scmRepositories]`

`[string]`

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`include`

`[string]`

Possible Values: `product, repository, xcodeVersion, macOsVersion`

## Response Codes

` 200 ``OK`

CiWorkflowsResponse

`OK`

The request completed successfully.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

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

Read the Xcode Cloud Product for an App

Get the Xcode Cloud product information for an app you build with Xcode Cloud.

