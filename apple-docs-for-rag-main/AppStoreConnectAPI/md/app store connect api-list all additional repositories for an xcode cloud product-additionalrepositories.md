

- App Store Connect API
-  List All Additional Repositories for an Xcode Cloud Product 

Web Service Endpoint

# List All Additional Repositories for an Xcode Cloud Product

List all additional Git repositories you associated with an Xcode Cloud product.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciProducts/{id}/additionalRepositories
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Products resource.

## Query Parameters

`fields[scmRepositories]`

`[string]`

Additional fields to include for each Repositories resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`filter[id]`

`[string]`

Filter the returned additional repositories using the ID of the Repositories resource.

`limit`

`integer`

The number of Repositories resources to return.

Maximum: `200`

`fields[scmGitReferences]`

`[string]`

Possible Values: `name, canonicalName, isDeleted, kind, repository`

`fields[scmProviders]`

`[string]`

Possible Values: `scmProviderType, url, repositories`

`include`

`[string]`

Possible Values: `scmProvider, defaultBranch`

## Response Codes

` 200 ``OK`

ScmRepositoriesResponse

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

