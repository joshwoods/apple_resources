

- App Store Connect API
-  Create a Beta App Localization 

Web Service Endpoint

# Create a Beta App Localization

Create localized descriptive information for an app.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaAppLocalizations
```

## HTTP Body

BetaAppLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaAppLocalizationResponse

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

## Overview

Important

A description is required for all `betaAppLocalizations` before you can submit to beta app review.

## See Also

### Creating, Modifying, and Deleting Localizations

Modify a Beta App Localization

Update the localized information for a specific beta app and locale.

Delete a Beta App Localization

Delete a beta app localization associated with an app.

