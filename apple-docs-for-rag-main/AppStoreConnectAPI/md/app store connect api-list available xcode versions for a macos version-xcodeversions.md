

- App Store Connect API
-  List Available Xcode Versions for a macOS Version 

Web Service Endpoint

# List Available Xcode Versions for a macOS Version

List all Xcode versions available for a specific macOS version in Xcode Cloud.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/{id}/xcodeVersions
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the macOS Versions resource.

## Query Parameters

`fields[ciMacOsVersions]`

`[string]`

Additional fields to include for each Xcode Versions resource returned by the response.

Possible Values: `version, name, xcodeVersions`

`fields[ciXcodeVersions]`

`[string]`

Additional fields to include for each Xcode Versions resource returned by the response.

Possible Values: `version, name, testDestinations, macOsVersions`

`include`

`[string]`

The relationship data to include in the response.

Value: `macOsVersions`

`limit`

`integer`

The number of Xcode Versions resources to return.

Maximum: `200`

`limit[macOsVersions]`

`integer`

The number of included Xcode Versions resources to return if the macOS versions relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

CiXcodeVersionsResponse

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

The example request below lists Xcode versions available in Xcode Cloud for a specific macOS version. Use the data provided in the response to display available Xcode versions and test destinations on a dashboard.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciMacOsVersions/20G95/xcodeVersions
```

```
{
    "data": [
        {
            "type": "ciXcodeVersions",
            "id": "Xcode12E507:stable",
            "attributes": {
                "version": "Xcode12E507:stable",
                "name": "Xcode 12.5.1 (12E507)",
                "testDestinations": [
                    {
                        "deviceTypeName": "iPhone 8",
                        "deviceTypeIdentifier": "com.apple.CoreSimulator.SimDeviceType.iPhone-8",
                        "availableRuntimes": [
                            {
                                "runtimeName": "iOS 13.0",
                                "runtimeIdentifier": "com.apple.CoreSimulator.SimRuntime.iOS-13-0"
                            }
                        ],
                        "kind": "SIMULATOR"
                    },
                    {
                        "deviceTypeName": "Mac",
                        "deviceTypeIdentifier": "mac",
                        "availableRuntimes": [
                            {
                                "runtimeName": "Same as Selected macOS Version",
                                "runtimeIdentifier": "builder"
                            },
                            {
                                "runtimeName": "Latest Beta or Release (Currently macOS Big Sur 11.5.2 (20G95))",
                                "runtimeIdentifier": "latest:all"
                            },
                            {
                                "runtimeName": "macOS Big Sur 11.5.2 (20G95)",
                                "runtimeIdentifier": "20G95"
                            }
                        ],
                        "kind": "MAC"
                    },
                    {
                        "deviceTypeName": "Mac (Mac Catalyst)",
                        "deviceTypeIdentifier": "mac_catalyst",
                        "availableRuntimes": [
                            {
                                "runtimeName": "Same as Selected macOS Version",
                                "runtimeIdentifier": "builder"
                            },
                            {
                                "runtimeName": "Latest Beta or Release (Currently macOS Big Sur 11.5.2 (20G95))",
                                "runtimeIdentifier": "latest:all"
                            },
                            {
                                "runtimeName": "macOS Big Sur 11.5.2 (20G95)",
                                "runtimeIdentifier": "20G95"
                            }
                        ],
                        "kind": "MAC"
                    }
                ]
            },
            "relationships": {
                "macOsVersions": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciXcodeVersions/Xcode12E507:stable/relationships/macOsVersions",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciXcodeVersions/Xcode12E507:stable/macOsVersions"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciXcodeVersions/Xcode20G95:stable"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciXcodeVersions"
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

### Getting macOS Version Information

List All macOS Versions Available in Xcode Cloud

List all macOS versions available to Xcode Cloud workflows.

Read macOS Version Information

Get information about a specific macOS version that’s available to Xcode Cloud workflows.

