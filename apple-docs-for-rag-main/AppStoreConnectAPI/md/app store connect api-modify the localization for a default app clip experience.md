

- App Store Connect API
-  Modify the Localization for a Default App Clip Experience 

Web Service Endpoint

# Modify the Localization for a Default App Clip Experience

Update localized metadata for a specific default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appClipDefaultExperienceLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experience Localizations resource.

## HTTP Body

AppClipDefaultExperienceLocalizationUpdateRequest

The request body you use to update a default App Clip experience localization.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppClipDefaultExperienceLocalizationResponse

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

### Managing Your Default App Clip Experience’s Metadata

Create the Localized Metadata for a Default App Clip Experience

Provide localized metadata that appears on the App Clip card of a default App Clip experience.

Delete a Default App Clip Experience Localization

Delete localized metadata that appears on the App Clip card of a default App Clip experience.

