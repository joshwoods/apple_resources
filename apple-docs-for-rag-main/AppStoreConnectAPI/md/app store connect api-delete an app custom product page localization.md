

- App Store Connect API
-  Delete an app custom product page localization 

Web Service Endpoint

# Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page localization resource ID from the List custom product pages localizations response.

## Response Codes

` 204 ``No Content`

`No Content`

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c
```

```
204
```

## See Also

### Endpoints

Create a custom product page localization

Add a localization for your app custom product page.

Modify custom product page localization information

Update the promotional text for an app custom product page localization.

List custom product pages localizations

List all localizations for an app custom product page.

Read custom product page localization information

Get information about a specific app custom product page localization.

List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

