

- App Store Connect API
-  Read macOS Version Information 

Web Service Endpoint

# Read macOS Version Information

Get information about a specific macOS version that’s available to Xcode Cloud workflows.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the macOS Versions resource.

## Query Parameters

`fields[ciMacOsVersions]`

`[string]`

Additional fields to include for the macOS Versions resource returned by the response.

Possible Values: `version, name, xcodeVersions`

`fields[ciXcodeVersions]`

`[string]`

Additional fields to include for the macOS Versions resource returned by the response.

Possible Values: `version, name, testDestinations, macOsVersions`

`include`

`[string]`

The relationship data to include in the response.

Value: `xcodeVersions`

`limit[xcodeVersions]`

`integer`

The number of included macOS Versions resources to return if the Xcode versions relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

CiMacOsVersionResponse

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

The example request below accesses information about a macOS version available to Xcode Cloud workflows. Use the data provided in the response to read additional information; for example, Xcode versions.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95
```

```
{
    "data": {
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
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95"
    }
}
```

## See Also

### Getting macOS Version Information

List All macOS Versions Available in Xcode Cloud

List all macOS versions available to Xcode Cloud workflows.

List Available Xcode Versions for a macOS Version

List all Xcode versions available for a specific macOS version in Xcode Cloud.

