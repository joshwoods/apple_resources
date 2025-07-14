

- App Store Connect API
-  Delete an App Store Version Localization 

Web Service Endpoint

# Delete an App Store Version Localization

Delete a language from your version metadata.

App Store Connect API 1.2+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

### Creating, Modifying, and Deleting Version Localizations

Create an App Store Version Localization

Add localized version-level information for a new locale.

Modify an App Store Version Localization

Modify localized version-level information for a particular language.

