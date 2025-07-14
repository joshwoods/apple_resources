

- App Store Connect API
-  Create a custom product page localization 

Web Service Endpoint

# Create a custom product page localization

Add a localization for your app custom product page.

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations
```

## HTTP Body

AppCustomProductPageLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppCustomProductPageLocalizationResponse

`Created`

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
POST https://appstoreconnect.apple.com/v1/appCustomProductPageLocalizations
{
    "data": {
        "type": "appCustomProductPageLocalizations",
        "attributes": {
            "locale": "en-CA",
            "promotionalText": "There will be so much fun."
        },
        "relationships": {
            "appCustomProductPageVersion": {
                "data": {
                    "type": "appCustomProductPageVersions",
                    "id": "46e3a412-7248-43f8-a6bf-cf445eafa3ef"
                }
            }
        }
    }
}
```

```
{
  "data" : {
    "type" : "appCustomProductPageLocalizations",
    "id" : "0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc",
    "attributes" : {
      "locale" : "en-CA",
      "promotionalText" : "There will be so much fun."
    },
    "relationships" : {
      "appScreenshotSets" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc/relationships/appScreenshotSets",
          "related" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc/appScreenshotSets"
        }
      },
      "appPreviewSets" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc/relationships/appPreviewSets",
          "related" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc/appPreviewSets"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0ff34f9c-e2f9-4317-a3e5-44e012c2ffbc"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations"
  }
}
```

## See Also

### Endpoints

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

Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

