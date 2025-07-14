

- App Store Connect API
-  Create a Routing App Coverage 

Web Service Endpoint

# Create a Routing App Coverage

Attach a routing app coverage file to an App Store version.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/routingAppCoverages
```

## HTTP Body

RoutingAppCoverageCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

RoutingAppCoverageResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Reading and Creating Routing App Coverages

Read the Routing App Coverage Information of an App Store Version

Get the routing app coverage file that is associated with a specific App Store version

Read Routing App Coverage Information

Get information about the routing app coverage file and its upload and processing status.

