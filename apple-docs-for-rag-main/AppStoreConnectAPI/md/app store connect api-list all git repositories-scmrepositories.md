

- App Store Connect API
-  List All Git Repositories 

Web Service Endpoint

# List All Git Repositories

List all Git repositories Xcode Cloud can access.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmRepositories
```

## Query Parameters

`fields[scmRepositories]`

`[string]`

Additional fields to include for each Repositories resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`filter[id]`

`[string]`

Filter the returned repositories using the ID of the Repositories resource.

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `scmProvider, defaultBranch`

`limit`

`integer`

The number of Repositories resources to return.

Maximum: `200`

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

## See Also

### Getting Repository Information

Read Git Repository Information

Get information about a Git repository that Xcode Cloud can access.

List All Git References for a Repository

List all Git references for a specific repository that Xcode Cloud can access.

List All Pull Requests for a Repository

List all pull requests for a specific repository that Xcode Cloud can access.

