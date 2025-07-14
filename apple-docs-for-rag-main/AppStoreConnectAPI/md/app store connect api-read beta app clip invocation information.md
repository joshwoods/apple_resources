

- App Store Connect API
-  Read Beta App Clip Invocation Information 

Web Service Endpoint

# Read Beta App Clip Invocation Information

Get a specific App Clip invocation you configure for testing.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaAppClipInvocations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Beta App Clip Invocations resource.

## Query Parameters

`fields[betaAppClipInvocations]`

`[string]`

Additional fields to include for each Beta App Clip Invocation resource returned by the response.

Possible Values: `url, betaAppClipInvocationLocalizations`

`include`

`[string]`

The relationship data to include in the response.

Value: `betaAppClipInvocationLocalizations`

`limit[betaAppClipInvocationLocalizations]`

`integer`

The number of included Beta App Clip Invocations resources to return if the beta App Clip invocation localizations relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

BetaAppClipInvocationResponse

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

## See Also

### Managing Beta App Clip Invocation

Create an App Clip Invocation for Testers in TestFlight

Configure a new App Clip experience that testers launch using the TestFlight app.

Modify an App Clip Invocation You Provide to Testers

Change an App Clip invocation you make available to testers in the TestFlight app.

Delete an App Clip Invocation for Testers in TestFlight

Delete an App Clip invocation you make available to testers in TestFlight.

