

- App Store Connect API
-  List app screenshot sets for a custom product page localization 

Web Service Endpoint

# List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/{id}/appScreenshotSets
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page localization resource ID from the List custom product pages localizations response.

## Query Parameters

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`fields[appScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, appScreenshotSet`

`filter[appStoreVersionExperimentTreatmentLocalization]`

`[string]`

`filter[appStoreVersionLocalization]`

`[string]`

`filter[screenshotDisplayType]`

`[string]`

Possible Values: `APP_IPHONE_67, APP_IPHONE_61, APP_IPHONE_65, APP_IPHONE_58, APP_IPHONE_55, APP_IPHONE_47, APP_IPHONE_40, APP_IPHONE_35, APP_IPAD_PRO_3GEN_129, APP_IPAD_PRO_3GEN_11, APP_IPAD_PRO_129, APP_IPAD_105, APP_IPAD_97, APP_DESKTOP, APP_WATCH_ULTRA, APP_WATCH_SERIES_10, APP_WATCH_SERIES_7, APP_WATCH_SERIES_4, APP_WATCH_SERIES_3, APP_APPLE_TV, APP_APPLE_VISION_PRO, IMESSAGE_APP_IPHONE_67, IMESSAGE_APP_IPHONE_61, IMESSAGE_APP_IPHONE_65, IMESSAGE_APP_IPHONE_58, IMESSAGE_APP_IPHONE_55, IMESSAGE_APP_IPHONE_47, IMESSAGE_APP_IPHONE_40, IMESSAGE_APP_IPAD_PRO_3GEN_129, IMESSAGE_APP_IPAD_PRO_3GEN_11, IMESSAGE_APP_IPAD_PRO_129, IMESSAGE_APP_IPAD_105, IMESSAGE_APP_IPAD_97`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`limit`

`integer`

Maximum: `200`

`limit[appScreenshots]`

`integer`

Maximum: `50`

`fields[appCustomProductPageLocalizations]`

`[string]`

Possible Values: `locale, promotionalText, appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionLocalizations]`

`[string]`

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

## Response Codes

` 200 ``OK`

AppScreenshotSetsResponse

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
https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/e0e9216a-338c-4616-9fd5-0ec6c14c6950/appCustomProductPageLocalizations
```

```
{
  "data": [
    {
      "type": "appScreenshotSets",
      "id": "3d87ecbb-bcdc-4c2f-b34f-ced3cf666de7",
      "attributes": {
        "screenshotDisplayType": "APP_IPHONE_65"
      },
      "relationships": {
        "appScreenshots": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/3d87ecbb-bcdc-4c2f-b34f-ced3cf666de7/relationships/appScreenshots",
            "related": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/3d87ecbb-bcdc-4c2f-b34f-ced3cf666de7/appScreenshots"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/3d87ecbb-bcdc-4c2f-b34f-ced3cf666de7"
      }
    },
    {
      "type": "appScreenshotSets",
      "id": "a59be7c9-8f97-45cc-939d-09c101c483e3",
      "attributes": {
        "screenshotDisplayType": "APP_IPHONE_55"
      },
      "relationships": {
        "appScreenshots": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/a59be7c9-8f97-45cc-939d-09c101c483e3/relationships/appScreenshots",
            "related": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/a59be7c9-8f97-45cc-939d-09c101c483e3/appScreenshots"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/a59be7c9-8f97-45cc-939d-09c101c483e3"
      }
    },
    {
      "type": "appScreenshotSets",
      "id": "69a9c45d-4508-4b4a-a08e-03e0bc018903",
      "attributes": {
        "screenshotDisplayType": "APP_IPAD_PRO_3GEN_129"
      },
      "relationships": {
        "appScreenshots": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/69a9c45d-4508-4b4a-a08e-03e0bc018903/relationships/appScreenshots",
            "related": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/69a9c45d-4508-4b4a-a08e-03e0bc018903/appScreenshots"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/69a9c45d-4508-4b4a-a08e-03e0bc018903"
      }
    },
    {
      "type": "appScreenshotSets",
      "id": "51bc2274-7517-4e56-82e4-c80f6014d44a",
      "attributes": {
        "screenshotDisplayType": "APP_IPAD_PRO_129"
      },
      "relationships": {
        "appScreenshots": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/51bc2274-7517-4e56-82e4-c80f6014d44a/relationships/appScreenshots",
            "related": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/51bc2274-7517-4e56-82e4-c80f6014d44a/appScreenshots"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appScreenshotSets/51bc2274-7517-4e56-82e4-c80f6014d44a"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/0d95bf9e-8256-4abf-83e2-9b428919100f/appScreenshotSets"
  },
  "meta": {
    "paging": {
      "total": 4,
      "limit": 50
    }
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

Read custom product page localization information

Get information about a specific app custom product page localization.

List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

