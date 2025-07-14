

- App Store Connect API
-  Read custom product page localization information 

Web Service Endpoint

# Read custom product page localization information

Get information about a specific app custom product page localization.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page localization resource ID from the List custom product pages localizations response.

## Query Parameters

`fields[appCustomProductPageLocalizations]`

`[string]`

Possible Values: `locale, promotionalText, appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`include`

`[string]`

Possible Values: `appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`limit[appPreviewSets]`

`integer`

Maximum: `50`

`limit[appScreenshotSets]`

`integer`

Maximum: `50`

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd
```

```
{
  "data": {
    "type": "appCustomProductPageLocalizations",
    "id": "dad51248-3c38-4f19-a814-3c4f6da719dd",
    "attributes": {
      "locale": "en-US",
      "promotionalText": "This app will inspire!"
    },
    "relationships": {
      "appScreenshotSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd/relationships/appScreenshotSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd/appScreenshotSets"
        }
      },
      "appPreviewSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd/relationships/appPreviewSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd/appPreviewSets"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/dad51248-3c38-4f19-a814-3c4f6da719dd"
  }
}
```

## See Also

### Endpoints

Create a custom product page localization

Add a localization for your app custom product page.

Modify custom product page localization information

Update the promotional text for an app custom product page localization.

List custom product pages localizations

List all localizations for an app custom product page.

List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

