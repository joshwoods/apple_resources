

- App Store Connect API
-  Create a Beta Build Localization 

Web Service Endpoint

# Create a Beta Build Localization

Create localized What’s New text for a build.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaBuildLocalizations
```

## HTTP Body

BetaBuildLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaBuildLocalizationResponse

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

### Creating, Modifying, and Deleting Beta Build Localizations

Modify a Beta Build Localization

Update the localized What’s New text for a specific beta build and locale.

Delete a Beta Build Localization

Delete a specific beta build localization associated with a build.

