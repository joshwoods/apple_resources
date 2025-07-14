

- App Store Connect API
-  List All Git References for a Repository 

Web Service Endpoint

# List All Git References for a Repository

List all Git references for a specific repository that Xcode Cloud can access.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmRepositories/{id}/gitReferences
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Repositories resource.

## Query Parameters

`fields[scmGitReferences]`

`[string]`

Additional fields to include for each Git References resource returned by the response.

Possible Values: `name, canonicalName, isDeleted, kind, repository`

`limit`

`integer`

The number of Git References resources to return.

Maximum: `200`

`fields[scmRepositories]`

`[string]`

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`include`

`[string]`

Value: `repository`

## Response Codes

` 200 ``OK`

ScmGitReferencesResponse

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

### Getting Repository Information

List All Git Repositories

List all Git repositories Xcode Cloud can access.

Read Git Repository Information

Get information about a Git repository that Xcode Cloud can access.

List All Pull Requests for a Repository

List all pull requests for a specific repository that Xcode Cloud can access.

