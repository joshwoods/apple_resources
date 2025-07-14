

- App Store Connect API
-  List custom product pages localizations 

Web Service Endpoint

# List custom product pages localizations

List all localizations for an app custom product page.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/{id}/appCustomProductPageLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page version resource ID from the List custom product page versions response.

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

`filter[locale]`

`[string]`

`include`

`[string]`

Possible Values: `appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`limit`

`integer`

Maximum: `200`

`limit[appPreviewSets]`

`integer`

Maximum: `50`

`limit[appScreenshotSets]`

`integer`

Maximum: `50`

`fields[appCustomProductPageVersions]`

`[string]`

Possible Values: `version, state, deepLink, appCustomProductPage, appCustomProductPageLocalizations`

## Response Codes

` 200 ``OK`

AppCustomProductPageLocalizationsResponse

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
https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/6c0df710-d69a-454f-be7c-f5b014788dee/appCustomProductPageLocalizations
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
}a{
  "data": [
    {
      "type": "appCustomProductPageLocalizations",
      "id": "77cefe66-a51a-4d4d-a5bd-cc40a733def0",
      "attributes": {
        "locale": "en-CA",
        "promotionalText": "This app will bring you inspiration."
      },
      "relationships": {
        "appScreenshotSets": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/77cefe66-a51a-4d4d-a5bd-cc40a733def0/relationships/appScreenshotSets",
            "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/77cefe66-a51a-4d4d-a5bd-cc40a733def0/appScreenshotSets"
          }
        },
        "appPreviewSets": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/77cefe66-a51a-4d4d-a5bd-cc40a733def0/relationships/appPreviewSets",
            "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/77cefe66-a51a-4d4d-a5bd-cc40a733def0/appPreviewSets"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/77cefe66-a51a-4d4d-a5bd-cc40a733def0"
      }
    },
    {
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
    {
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
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/6c0df710-d69a-454f-be7c-f5b014788dee/appCustomProductPageLocalizations"
  },
  "meta": {
    "paging": {
      "total": 3,
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

Read custom product page localization information

Get information about a specific app custom product page localization.

List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

Delete an app custom product page localization

Delete localized metadata that you configured for a custom product page.

