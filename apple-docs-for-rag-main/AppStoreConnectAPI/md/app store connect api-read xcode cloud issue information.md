

- App Store Connect API
-  Read Xcode Cloud Issue Information 

Web Service Endpoint

# Read Xcode Cloud Issue Information

Get information about a specific issue that occurred when Xcode Cloud performed a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciIssues/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Issues resource.

## Query Parameters

`fields[ciIssues]`

`[string]`

Additional fields to include for the Issues resource returned by the response.

Possible Values: `issueType, message, fileSource, category`

## Response Codes

` 200 ``OK`

CiIssueResponse

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

The example request below retrieves information about a specific issue Xcode Cloud encountered when it performed a build. Use the information provided to display issues on a dashboard, create reports, and so on.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciIssues/61473b34-2ecd-498d-9e2b-94216b7e8fb4
```

```
{
    "data": {
        "type": "ciIssues",
        "id": "61473b34-2ecd-498d-9e2b-94216b7e8fb4",
        "attributes": {
            "issueType": "ERROR",
            "message": "A message describing the issue.",
            "fileSource": {
                "path": "/the/path/to/the/file/with/the/issue",
                "lineNumber": 42
            },
            "category": null
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciIssues/61473b34-2ecd-498d-9e2b-94216b7e8fb4"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciIssues/61473b34-2ecd-498d-9e2b-94216b7e8fb4"
    }
}
```

