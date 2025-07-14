

- App Store Connect API
-  Read Pull Request Information 

Web Service Endpoint

# Read Pull Request Information

Get information about a specific pull request.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmPullRequests/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Pull Requests resource.

## Query Parameters

`fields[scmPullRequests]`

`[string]`

Additional fields to include for the Pull Requests resource returned by the response.

Possible Values: `title, number, webUrl, sourceRepositoryOwner, sourceRepositoryName, sourceBranchName, destinationRepositoryOwner, destinationRepositoryName, destinationBranchName, isClosed, isCrossRepository, repository`

`include`

`[string]`

The relationship data to include in the response.

Value: `repository`

## Response Codes

` 200 ``OK`

ScmPullRequestResponse

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

The example request below retrieves information about a specific pull request. For example, use the data provided in the response to display pull request information on a custom dashboard.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/scmPullRequests/3372ba3b-013d-4328-9b48-0ef8ec54f48d
```

```
{
    "data": {
        "type": "scmPullRequests",
        "id": "3372ba3b-013d-4328-9b48-0ef8ec54f48d",
        "attributes": {
            "title": "A sample pull request",
            "number": 123,
            "webUrl": "https://github.com/example-user/example-app/pull/123",
            "sourceRepositoryOwner": "example-user",
            "sourceRepositoryName": "example-app",
            "sourceBranchName": "BRANCH",
            "destinationRepositoryOwner": "example-user",
            "destinationRepositoryName": "example-app",
            "destinationBranchName": "main",
            "isClosed": false,
            "isCrossRepository": false
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/scmPullRequests/3372ba3b-013d-4328-9b48-0ef8ec54f48d"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/scmPullRequests/3372ba3b-013d-4328-9b48-0ef8ec54f48d"
    }
}
```

