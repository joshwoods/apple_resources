

- App Store Connect API
-  Modify an App Info 

Web Service Endpoint

# Modify an App Info

Update the App Store categories and sub-categories for your app.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appInfos/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

AppInfoUpdateRequest

The request body you use to update an App Info.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppInfoResponse

`OK`

Request succeeded.

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

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Use this endpoint to modify the primary and secondary categories and subcategories for an app.

### Add an App to the Games Category and the Sports and Role Playing Subcategories

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4

{
  "data": {
    "type": "appInfos",
    "id": "61d77dc2-9313-4330-b169-d179277ccfc4",
    "relationships": {
      "primaryCategory": {
        "data": {
          "type": "appCategories",
          "id": "GAMES"
        }
      },
      "primarySubcategoryOne": {
        "data": {
          "type": "appCategories",
          "id": "GAMES_SPORTS"
        }
      },
      "primarySubcategoryTwo": {
        "data": {
          "type": "appCategories",
          "id": "GAMES_ROLE_PLAYING"
        }
      }
    }
  }
}

```

```
{
  "data": {
    "type": "appInfos",
    "id": "61d77dc2-9313-4330-b169-d179277ccfc4",
    "attributes": {
      "appStoreState": "READY_FOR_SALE",
      "appStoreAgeRating": "TWELVE_PLUS",
      "brazilAgeRating": "FOURTEEN",
      "kidsAgeBand": null
    },
    "relationships": {
      "app": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/app",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/app"
        }
      },
      "appInfoLocalizations": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/appInfoLocalizations",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/appInfoLocalizations"
        }
      },
      "primaryCategory": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/primaryCategory",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/primaryCategory"
        }
      },
      "primarySubcategoryOne": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/primarySubcategoryOne",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/primarySubcategoryOne"
        }
      },
      "primarySubcategoryTwo": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/primarySubcategoryTwo",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/primarySubcategoryTwo"
        }
      },
      "secondaryCategory": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/secondaryCategory",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/secondaryCategory"
        }
      },
      "secondarySubcategoryOne": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/secondarySubcategoryOne",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/secondarySubcategoryOne"
        }
      },
      "secondarySubcategoryTwo": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/relationships/secondarySubcategoryTwo",
          "related": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4/secondarySubcategoryTwo"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appInfos/61d77dc2-9313-4330-b169-d179277ccfc4"
  }
}

```

