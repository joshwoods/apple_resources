

- App Store Connect API
-  Delete a Beta Group 

Web Service Endpoint

# Delete a Beta Group

Delete a beta group and remove beta tester access to associated builds.

App Store Connect API 1.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/betaGroups/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Creating, Modifying, and Deleting Beta Groups

Create a Beta Group

Create a beta group associated with an app, optionally enabling TestFlight public links.

Modify a Beta Group

Modify a beta group’s metadata, including changing its Testflight public link status.

