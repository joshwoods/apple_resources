

- App Store Connect API
-  Modify a Routing App Coverage 

Web Service Endpoint

# Modify a Routing App Coverage

Commit a routing app coverage file after uploading it.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/routingAppCoverages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

RoutingAppCoverageUpdateRequest

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Modifying and Deleting Routing App Coverages

Delete a Routing App Coverage

Delete the routing app coverage file that is associated with a version.

