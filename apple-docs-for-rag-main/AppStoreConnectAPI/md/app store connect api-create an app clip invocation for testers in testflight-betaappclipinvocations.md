

- App Store Connect API
-  Create an App Clip Invocation for Testers in TestFlight 

Web Service Endpoint

# Create an App Clip Invocation for Testers in TestFlight

Configure a new App Clip experience that testers launch using the TestFlight app.

App Store Connect API 1.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaAppClipInvocations
```

## HTTP Body

BetaAppClipInvocationCreateRequest

The request body you use to create a beta App Clip invocation.

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaAppClipInvocationResponse

`Created`

The request completed successfully and a new Beta App Clip Invocations resource has been created.

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

### Managing Beta App Clip Invocation

Read Beta App Clip Invocation Information

Get a specific App Clip invocation you configure for testing.

Modify an App Clip Invocation You Provide to Testers

Change an App Clip invocation you make available to testers in the TestFlight app.

Delete an App Clip Invocation for Testers in TestFlight

Delete an App Clip invocation you make available to testers in TestFlight.

