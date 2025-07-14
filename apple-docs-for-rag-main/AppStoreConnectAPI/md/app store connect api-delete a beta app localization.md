

- App Store Connect API
-  Delete a Beta App Localization 

Web Service Endpoint

# Delete a Beta App Localization

Delete a beta app localization associated with an app.

App Store Connect API 1.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/betaAppLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

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

### Creating, Modifying, and Deleting Localizations

Create a Beta App Localization

Create localized descriptive information for an app.

Modify a Beta App Localization

Update the localized information for a specific beta app and locale.

