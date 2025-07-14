

- App Store Connect API
-  Modify Localized Metadata of an App Clip Invocation for Testers 

Web Service Endpoint

# Modify Localized Metadata of an App Clip Invocation for Testers

Change the metadata for an App Clip you make available to testers in the TestFlight app.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/betaAppClipInvocationLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Beta App Clip Invocation Localizations resource.

## HTTP Body

BetaAppClipInvocationLocalizationUpdateRequest

The request body you use to update a beta App Clip invocation localization.

Content-Type: application/json

## Response Codes

` 200 ``OK`

BetaAppClipInvocationLocalizationResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing Localizations for Invocations of Beta App Clips

Create Localized Metadata for a Beta App Clip Invocation

Provide localized metadata for an App Clip experience you make available to testers.

Delete a Beta App Clip Invocation Localization

Delete localized metadata you configured for an App Clip that testers launch using the TestFlight app.

