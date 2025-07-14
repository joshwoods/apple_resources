

- App Store Connect API
-  Read Routing App Coverage Information 

Web Service Endpoint

# Read Routing App Coverage Information

Get information about the routing app coverage file and its upload and processing status.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/routingAppCoverages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[routingAppCoverages]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreVersion`

`include`

`[string]`

Value: `appStoreVersion`

## Response Codes

` 200 ``OK`

RoutingAppCoverageResponse

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

### Reading and Creating Routing App Coverages

Read the Routing App Coverage Information of an App Store Version

Get the routing app coverage file that is associated with a specific App Store version

Create a Routing App Coverage

Attach a routing app coverage file to an App Store version.

