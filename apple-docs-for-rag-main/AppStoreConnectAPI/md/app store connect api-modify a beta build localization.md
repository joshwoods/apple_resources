

- App Store Connect API
-  Modify a Beta Build Localization 

Web Service Endpoint

# Modify a Beta Build Localization

Update the localized What’s New text for a specific beta build and locale.

App Store Connect API 1.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/betaBuildLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BetaBuildLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

BetaBuildLocalizationResponse

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

### Creating, Modifying, and Deleting Beta Build Localizations

Create a Beta Build Localization

Create localized What’s New text for a build.

Delete a Beta Build Localization

Delete a specific beta build localization associated with a build.

