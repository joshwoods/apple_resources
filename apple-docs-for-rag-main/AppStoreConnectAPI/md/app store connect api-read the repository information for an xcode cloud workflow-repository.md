

- App Store Connect API
-  Read the Repository Information for an Xcode Cloud Workflow 

Web Service Endpoint

# Read the Repository Information for an Xcode Cloud Workflow

Get information about the Git repository of a specific Xcode Cloud workflow.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciWorkflows/{id}/repository
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Workflows resource.

## Query Parameters

`fields[scmRepositories]`

`[string]`

Additional fields to include for the Repositories resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

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

The example request below retrieves information about an Xcode Cloud workflow’s repository. Use the data provided in the response to read additional information; for example, pull request information.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/repository
```

```
{
    "data": {
      "type": "scmRepositories",
      "id": "a2b04ba9-85fa-478c-87a2-b6d19626b870",
      "attributes": {
        "lastAccessedDate": null,
        "httpCloneUrl": "https://github.com/foo/bar.git",
        "sshCloneUrl": "ssh://git@github.com/foo/bar.git",
        "ownerName": "foo",
        "repositoryName": "bar"
      },
      "relationships": {
        "gitReferences": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/relationships/gitReferences",
            "related": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/gitReferences"
          }
        },
        "pullRequests": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/relationships/pullRequests",
            "related": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870/pullRequests"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870"
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/scmRepositories/a2b04ba9-85fa-478c-87a2-b6d19626b870"
    }
}
```

## See Also

### Getting Xcode Cloud Workflows

Read Xcode Cloud Workflow Information

Get information about a specific Xcode Cloud workflow.

List All Xcode Cloud Builds for a Workflow

List all builds Xcode Cloud performed for a specific workflow.

