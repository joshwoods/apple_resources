

- App Store Connect API
-  Read the Routing App Coverage Information of an App Store Version 

Web Service Endpoint

# Read the Routing App Coverage Information of an App Store Version

Get the routing app coverage file that is associated with a specific App Store version

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/routingAppCoverage
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[routingAppCoverages]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreVersion`

## Response Codes

` 200 ``OK`

RoutingAppCoverageWithoutIncludesResponse

`OK`

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

## See Also

### Reading Declarations

Read the Age Rating Declaration Information of an App Store Version

Get the age-related information declared for your app.

Deprecated

