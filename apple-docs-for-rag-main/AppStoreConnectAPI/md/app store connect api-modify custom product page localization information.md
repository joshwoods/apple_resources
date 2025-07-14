

- App Store Connect API
-  Modify custom product page localization information 

Web Service Endpoint

# Modify custom product page localization information

Update the promotional text for an app custom product page localization.

App Store Connect API 1.7+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page localization resource ID from the List custom product pages localizations response.

## HTTP Body

AppCustomProductPageLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppCustomProductPageLocalizationResponse

`OK`

Content-Type: application/json

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

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c
{
    "data": {
        "id": "736966e2-178b-4e3f-bfb9-474eb19fbd8c",
        "type": "appCustomProductPageLocalizations",
        "attributes": {
            "promotionalText": "Ogenblik!"
        }
    }
}
```

```
{
  "data": {
    "type": "appCustomProductPageLocalizations",
    "id": "736966e2-178b-4e3f-bfb9-474eb19fbd8c",
    "attributes": {
      "locale": "nl-NL",
      "promotionalText": "Ogenblik!"
    },
    "relationships": {
      "appScreenshotSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c/relationships/appScreenshotSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c/appScreenshotSets"
        }
      },
      "appPreviewSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c/relationships/appPreviewSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c/appPreviewSets"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/736966e2-178b-4e3f-bfb9-474eb19fbd8c"
  }
}
```

## See Also

### Endpoints

Create a custom product page localization

Add a localization for your app custom product page.

List custom product pages localizations

List all localizations for an app custom product page.

Read custom product page localization information

Get information about a specific app custom product page localization.

List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

