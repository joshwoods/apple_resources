

- App Store Connect API
-  Create an App Info Localization 

Web Service Endpoint

# Create an App Info Localization

Add app-level localized information for a new locale.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appInfoLocalizations
```

## HTTP Body

AppInfoLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppInfoLocalizationResponse

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

## Mentioned in 

App Store Connect API 3.7 release notes

## Discussion

Use this endpoint to add localized app information for a new locale. Be sure to use Create an App Store Version Localization to add the same locale to the version as well.

Important

If the app store version and the app info don’t have the same set of localizations, you will receive an erorr when you submit the version to the App Store.

### Add Localized App Information in US English

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/appInfoLocalizations

{
  "data": {
    "type": "appInfoLocalizations",
    "attributes": {
      "locale": "en-US",
      "name": "Forest Explorer",
      "subtitle": "Hikes, trails, and maps",
      "privacyPolicyUrl": "http://forestexplorer.apple.com/privacy-simple"
    },
    "relationships": {
      "appInfo": {
        "data": {
          "type": "appInfos",
          "id": "9c8e7e2b-07a8-45d9-8951-948507275bc6"
        }
      }
    }
  }
}
```

```
{
  "data": {
    "type": "appInfoLocalizations",
    "id": "9c8e7e2b-07a8-45d9-8951-948507275bc6",
    "attributes": {
      "locale": "en-GB",
      "name": "Forest Explorer",
      "subtitle": "Hikes, trails, and maps",
      "privacyPolicyUrl": "http://forestexplorer.apple.com/privacy-simple",
      "privacyPolicyText": null
    },
    "relationships": {
      "appInfo": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/74ae3739-d321-4f83-afc3-3b66043ff163/relationships/appInfo",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/74ae3739-d321-4f83-afc3-3b66043ff163/appInfo"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/74ae3739-d321-4f83-afc3-3b66043ff163"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/74ae3739-d321-4f83-afc3-3b66043ff163"
  }
}
```

## See Also

### Creating, Modifying, and Deleting Localized App Information

Modify an App Info Localization

Modify localized app-level information for a particular language.

Delete an App Info Localization

Delete an app information localization that is associated with an app.

