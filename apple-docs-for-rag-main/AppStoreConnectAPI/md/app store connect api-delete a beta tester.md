

- App Store Connect API
-  Delete a Beta Tester 

Web Service Endpoint

# Delete a Beta Tester

Remove a beta tester’s ability to test all apps.

App Store Connect API 1.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/betaTesters/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Response Codes

` 202 ``Accepted`

`Accepted`

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

### Creating and Deleting Beta Testers

Create a Beta Tester

Create a beta tester assigned to a group, a build, or an app.

