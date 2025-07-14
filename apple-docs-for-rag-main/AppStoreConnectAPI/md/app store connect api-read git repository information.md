

- App Store Connect API
-  Read Git Repository Information 

Web Service Endpoint

# Read Git Repository Information

Get information about a Git repository that Xcode Cloud can access.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmRepositories/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Repositories resource.

## Query Parameters

`fields[scmRepositories]`

`[string]`

Additional fields to include for the Repositories resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `scmProvider, defaultBranch`

## Response Codes

` 200 ``OK`

ScmRepositoryResponse

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

## Discussion

The example request below retrieves information about a specific Git repository that Xcode Cloud can access. Use the data provided in the response to read additional information; for example, pull request information.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870
```

```
{
    “data”: {
      “type”: “scmRepositories”,
      “id”: “a2b04ba9-85fa-478c-87a2-b6d19626b870”,
      “attributes”: {
        “lastAccessedDate”: null,
        “httpCloneUrl”: “https://github.com/foo/bar.git”,
        “sshCloneUrl”: “ssh://git@github.com/foo/bar.git”,
        “ownerName”: “foo”,
        “repositoryName”: “bar”
      },
      “relationships”: {
        “gitReferences”: {
          “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/relationships/gitReferences”,
            “related”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/gitReferences”
          }
        },
        “pullRequests”: {
          “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/relationships/pullRequests”,
            “related”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/pullRequests”
          }
        }
      },
      “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870”
      }
    },
    “links”: {
      “self”: “https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870”
    }
  }
```

## See Also

### Getting Repository Information

List All Git Repositories

List all Git repositories Xcode Cloud can access.

List All Git References for a Repository

List all Git references for a specific repository that Xcode Cloud can access.

List All Pull Requests for a Repository

List all pull requests for a specific repository that Xcode Cloud can access.

