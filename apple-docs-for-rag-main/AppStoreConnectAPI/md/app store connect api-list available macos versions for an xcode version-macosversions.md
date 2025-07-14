

- App Store Connect API
-  List Available macOS Versions for an Xcode Version 

Web Service Endpoint

# List Available macOS Versions for an Xcode Version

List all macOS versions available in Xcode Cloud that support a specific Xcode version.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciXcodeVersions/{id}/macOsVersions
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Xcode Versions resource.

## Query Parameters

`fields[ciMacOsVersions]`

`[string]`

Additional fields to include for each macOS Versions resource returned by the response.

Possible Values: `version, name, xcodeVersions`

`fields[ciXcodeVersions]`

`[string]`

Additional fields to include for each macOS Versions resource returned by the response.

Possible Values: `version, name, testDestinations, macOsVersions`

`include`

`[string]`

The relationship data to include in the response.

Value: `xcodeVersions`

`limit`

`integer`

The number of macOS Versions resources to return.

Maximum: `200`

`limit[xcodeVersions]`

`integer`

The number of included macOS Versions resources to return if the Xcode versions relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

CiMacOsVersionsResponse

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

The example request below lists macOS versions available for a specific Xcode version. Use the information provided in the response to update workflows, build dashboards, and more.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciXcodeVersions/b1e1f7b2-14e7-11ec-82a8-0242ac130003/macOsVersions
```

```
{
    "data": [
        {
            "type": "ciMacOsVersions",
            "id": "20G95",
            "attributes": {
                "version": "20G95",
                "name": "macOS Big Sur 11.5.2 (20G95)"
            },
            "relationships": {
                "xcodeVersions": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95/relationships/xcodeVersions",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95/xcodeVersions"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciMacOsVersions"
    },
    "meta": {
        "paging": {
            "total": 1,
            "limit": 50
        }
    }
}
```

## See Also

### Getting Xcode Version Information

List All Xcode Versions Available in Xcode Cloud

List all Xcode versions that are available to Xcode Cloud workflows.

Read Xcode Version Information

Get information about a specific Xcode version that’s available to Xcode Cloud workflows.

