

- App Store Connect API
-  Modify an App Info Localization 

Web Service Endpoint

# Modify an App Info Localization

Modify localized app-level information for a particular language.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppInfoLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppInfoLocalizationResponse

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

### Creating, Modifying, and Deleting Localized App Information

Create an App Info Localization

Add app-level localized information for a new locale.

Delete an App Info Localization

Delete an app information localization that is associated with an app.

