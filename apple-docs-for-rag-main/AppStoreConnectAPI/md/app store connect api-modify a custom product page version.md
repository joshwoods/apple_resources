

- App Store Connect API
-  Modify a custom product page version 

Web Service Endpoint

# Modify a custom product page version

Update the name and visibility status of an app custom product page.

App Store Connect API 3.5+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page version resource ID from the List custom product page versions response.

## HTTP Body

AppCustomProductPageVersionUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppCustomProductPageVersionResponse

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
PATCH https://appstoreconnect.apple.com/v1/appCustomProductPageVersions/372e5398-047b-4793-951b-2935d8578ab2
{
    "data": {
        "type": "appCustomProductPageVersions",
        "id": "372e5398-047b-4793-951b-2935d8578ab2",
        "attributes": {
            "deepLink": "https://example.com/deeplink"
        }
    }
}
```

```
{
  "data" : {
    "type" : "appCustomProductPageVersions",
    "id" : "372e5398-047b-4793-951b-2935d8578ab2",
    "attributes" : {
      "version" : "3",
      "state" : "PREPARE_FOR_SUBMISSION",
      "deepLink" : "https://example.com/deeplink"
    },
    "relationships" : {
      "appCustomProductPageLocalizations" : {
        "links" : {
          "self" : "https://appstoreconnect.apple.com/v1/appCustomProductPageVersions/372e5398-047b-4793-951b-2935d8578ab2/relationships/appCustomProductPageLocalizations",
          "related" : "https://appstoreconnect.apple.com/v1/appCustomProductPageVersions/372e5398-047b-4793-951b-2935d8578ab2/appCustomProductPageLocalizations"
        }
      }
    },
    "links" : {
      "self" : "https://appstoreconnect.apple.com/v1/appCustomProductPageVersions/372e5398-047b-4793-951b-2935d8578ab2"
    }
  },
  "links" : {
    "self" : "https://appstoreconnect.apple.com/v1/appCustomProductPageVersions/372e5398-047b-4793-951b-2935d8578ab2"
  }
}
```

## See Also

### Endpoints

Read custom product page version information

Get information about a specific app custom product page version.

List custom product page versions

List the versions for a custom product page version.

List custom product pages localizations

List all localizations for an app custom product page.

Create a custom product page version

Add a version for your app custom product page.

