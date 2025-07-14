

- App Store Connect API
-  List all Repositories for a Source Code Management Provider 

Web Service Endpoint

# List all Repositories for a Source Code Management Provider

List all Git repositories for a specific source code management provider you connected to Xcode Cloud.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmProviders/{id}/repositories
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Providers resource.

## Query Parameters

`fields[scmRepositories]`

`[string]`

Additional fields to include for each Repositories resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`filter[id]`

`[string]`

Filter the returned repositories using the ID of the Repositories resource.

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

### Getting Provider Information

List All Source Code Management Providers

List all source code management providers you connected to Xcode Cloud.

Get a Source Code Management Provider

Get information about a specific source code management provider you connected to Xcode Cloud.

