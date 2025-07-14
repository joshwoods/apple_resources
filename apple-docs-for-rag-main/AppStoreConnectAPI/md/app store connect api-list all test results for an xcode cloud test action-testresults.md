

- App Store Connect API
-  List All Test Results for an Xcode Cloud Test Action 

Web Service Endpoint

# List All Test Results for an Xcode Cloud Test Action

List all test results for a specific test action Xcode Cloud performed as part of a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/{id}/testResults
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Actions resource.

## Query Parameters

`fields[ciTestResults]`

`[string]`

Additional fields to include for each Test Results resource returned by the response.

Possible Values: `className, name, status, fileSource, message, destinationTestResults`

`limit`

`integer`

The number of Test Results resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

CiTestResultsResponse

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

The example request below lists the test results for an Xcode Cloud build that performed a test action. Use the information provided in the response to display test results on a dashboard, create a new task for a failing test in your issue tracker, and so on.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/d871dabb-2c2c-4012-aff5-abb427bcb3a3/testResults
```

```
{
"data": [
        {
            "type": "ciTestResults",
            "id": "87f8a597-bea9-49d8-ba8b-6a643de66903",
            "attributes": {
                "className": "TestClass",
                "name": "TestName",
                "status": "SUCCESS",
                "fileSource": {
                    "path": "path",
                    "lineNumber": 100
                },
                "message": null,
                "destinationTestResults": [
                    {
                        "uuid": "8d1bff05-2b9c-4cc4-9225-e2cd41dee260",
                        "deviceName": "iPhone X",
                        "osVersion": "11.4.1",
                        "status": "SUCCESS",
                        "duration": 6.600471973
                    }
                ]
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciTestResults/87f8a597-bea9-49d8-ba8b-6a643de66903"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/d871dabb-2c2c-4012-aff5-abb427bcb3a3/testResults"
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

List All Issues for a Build Action

List all issues that occurred for a specific action that Xcode Cloud performed as part of a build.

