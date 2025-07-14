

- App Store Connect API
-  Read Test Result Information 

Web Service Endpoint

# Read Test Result Information

Get a specific test result Xcode Cloud created when it performed a build with a test action.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciTestResults/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Test Results resource.

## Query Parameters

`fields[ciTestResults]`

`[string]`

Additional fields to include for the Test Results resource returned by the response.

Possible Values: `className, name, status, fileSource, message, destinationTestResults`

## Response Codes

` 200 ``OK`

CiTestResultResponse

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

The example request below retrieves result information for a test Xcode Cloud performed. Use the data provided in the response to display test result information on a dashboard, create reports, or create a new issue in your issue tracker for a failing test.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciTestResults/5ecb25ea-ce31-4b50-b88c-f1bf64c698ae
```

```
{
    "data": {
        "type": "ciTestResults",
        "id": "5ecb25ea-ce31-4b50-b88c-f1bf64c698ae",
        "attributes": {
            "className": "TestClass",
            "name": "TestName",
            "status": "SUCCESS",
            "fileSource": null,
            "message": null,
            "destinationTestResults": [
                {
                    "uuid": "e456c6a3-37a3-42c7-8299-33dad720f6b7",
                    "deviceName": "iPhone X",
                    "osVersion": "11.4.1",
                    "status": "SUCCESS",
                    "duration": 6.600471973
                }
            ]
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciTestResults/5ecb25ea-ce31-4b50-b88c-f1bf64c698ae"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciTestResults/5ecb25ea-ce31-4b50-b88c-f1bf64c698ae"
    }
}
```

