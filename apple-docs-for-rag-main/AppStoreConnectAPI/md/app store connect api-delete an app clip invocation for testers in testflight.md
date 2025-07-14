

- App Store Connect API
-  Delete an App Clip Invocation for Testers in TestFlight 

Web Service Endpoint

# Delete an App Clip Invocation for Testers in TestFlight

Delete an App Clip invocation you make available to testers in TestFlight.

App Store Connect API 1.6+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/betaAppClipInvocations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Beta App Clip Invocations resource.

## Response Codes

` 204 ``No Content`

`No Content`

The request completed successfully and the specific Beta App Clip Invocations resource was deleted.

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

### Managing Beta App Clip Invocation

Read Beta App Clip Invocation Information

Get a specific App Clip invocation you configure for testing.

Create an App Clip Invocation for Testers in TestFlight

Configure a new App Clip experience that testers launch using the TestFlight app.

Modify an App Clip Invocation You Provide to Testers

Change an App Clip invocation you make available to testers in the TestFlight app.

