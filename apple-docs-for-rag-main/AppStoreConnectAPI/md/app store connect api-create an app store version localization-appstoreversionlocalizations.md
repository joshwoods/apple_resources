

- App Store Connect API
-  Create an App Store Version Localization 

Web Service Endpoint

# Create an App Store Version Localization

Add localized version-level information for a new locale.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations
```

## HTTP Body

AppStoreVersionLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionLocalizationResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Use this endpoint to add localized version information for a new locale. Be sure to use Create an App Info Localization to add the same locale to the version as well.

Important

If the app store version and the app info don’t have the same set of localizations, you will receive an erorr when you submit the version to the App Store.

### Add Localized App Store Version Information in US English

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations

{
  "data": {
    "type": "appStoreVersionLocalizations",
    "attributes": {
      "locale": "en-US",
      "description": "Go wild and discover trails, parks and off-the-beaten-track terrain with Forest Explorer. Whether you’re bushwalking in the outback or looking for a quick local hike, Forest Explorer has thousands of trails and destinations from around the globe to explore.",
      "keywords": "hiking, trails, backcountry, parks, path, terrain, forest",
      "marketingUrl": "http://www.apple.com/forestexplorer",
      "promotionalText": "Get Forest Explorer free for a limited time.",
      "supportUrl": "https://support.apple.com",
      "whatsNew": "Now includes trails in Europe and South America"
    },
    "relationships": {
      "appStoreVersion": {
        "data": {
          "type": "appStoreVersions",
          "id": "54457681-4b65-4071-a636-ea66cb98c8e9"
        }
      }
    }
  }
}
```

```
{
  "data": {
    "type": "appStoreVersionLocalizations",
    "id": "af806ced-8826-4a9d-8a0f-9f3402ce3629",
    "attributes": {
      "locale": "en-US",
      "description": "Go wild and discover trails, parks and off-the-beaten-track terrain with Forest Explorer. Whether you’re bushwalking in the outback or looking for a quick local hike, Forest Explorer has thousands of trails and destinations from around the globe to explore.",
      "keywords": "hiking, trails, backcountry, parks, path, terrain, forest",
      "marketingUrl": "http://www.apple.com/forestexplorer",
      "promotionalText": "Get Forest Explorer free for a limited time.",
      "supportUrl": "https://support.apple.com",
      "whatsNew": "Now includes trails in Europe and South America"
    },
    "relationships": {
      "appStoreVersion": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/relationships/appStoreVersion",
          "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/appStoreVersion"
        }
      },
      "appScreenshotSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/relationships/appScreenshotSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/appScreenshotSets"
        }
      },
      "appPreviewSets": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/relationships/appPreviewSets",
          "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629/appPreviewSets"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/af806ced-8826-4a9d-8a0f-9f3402ce3629"
  }
}

```

## See Also

### Creating, Modifying, and Deleting Version Localizations

Modify an App Store Version Localization

Modify localized version-level information for a particular language.

Delete an App Store Version Localization

Delete a language from your version metadata.

