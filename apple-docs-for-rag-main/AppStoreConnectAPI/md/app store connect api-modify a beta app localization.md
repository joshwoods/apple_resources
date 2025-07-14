

- App Store Connect API
-  Modify a Beta App Localization 

Web Service Endpoint

# Modify a Beta App Localization

Update the localized information for a specific beta app and locale.

App Store Connect API 1.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/betaAppLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `betaAppLocalizations` resource ID from the List Beta App Localizations response.

## HTTP Body

BetaAppLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

BetaAppLocalizationResponse

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

## Mentioned in 

App Store Connect API 3.7 release notes

## Overview

Important

A description is required for all `betaAppLocalizations` before you can submit to beta app review. After you have added data to the fields for this resource, you can change that data, but you cannot remove data.

## See Also

### Creating, Modifying, and Deleting Localizations

Create a Beta App Localization

Create localized descriptive information for an app.

Delete a Beta App Localization

Delete a beta app localization associated with an app.

