

- App Store Connect API
-  List All Issues for a Build Action 

Web Service Endpoint

# List All Issues for a Build Action

List all issues that occurred for a specific action that Xcode Cloud performed as part of a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/{id}/issues
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Actions resource.

## Query Parameters

`fields[ciIssues]`

`[string]`

Additional fields to include for each Issues resource returned by the response.

Possible Values: `issueType, message, fileSource, category`

`limit`

`integer`

The number of Issues resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

CiIssuesResponse

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

The example request below lists all issues Xcode Cloud encountered when it performed a build. Use the information provided in the response to display issue information on a dashboard, generate reports, automatically create tasks in your issue tracker, and so on.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/2488c5ec-ee0c-425e-902b-41c1e88208ca/issues
```

```
{
"data": [
        {
            "type": "ciIssues",
            "id": "b5ed3706-96e4-4111-be17-049fb365b72e",
            "attributes": {
                "issueType": "ERROR",
                "message": "An example message.",
                "fileSource": {
                    "path": "/path/to/the/file/that/contains/the/issue",
                    "lineNumber": 42
                },
                "category": null
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciIssues/b5ed3706-96e4-4111-be17-049fb365b72e"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/2488c5ec-ee0c-425e-902b-41c1e88208ca/issues"
    },
    "meta": {
        "paging": {
            "limit": 50
        }
    }
}
```

## See Also

### Getting Build Actions

Read Build Action Information

Get information about a specific action Xcode Cloud performed as part of a build.

List All Artifacts for a Build Action

List all artifacts Xcode Cloud created when it performed an action.

Read the Xcode Cloud Build Information for a Build Action

Get Xcode Cloud build information for a given build action.

List All Test Results for an Xcode Cloud Test Action

List all test results for a specific test action Xcode Cloud performed as part of a build.

