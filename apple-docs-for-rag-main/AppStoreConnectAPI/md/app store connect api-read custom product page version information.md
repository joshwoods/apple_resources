

- App Store Connect API
-  Read custom product page version information 

Web Service Endpoint

# Read custom product page version information

Get information about a specific app custom product page version.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/{id}
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

`fields[appCustomProductPageVersions]`

`[string]`

Possible Values: `version, state, deepLink, appCustomProductPage, appCustomProductPageLocalizations`

`include`

`[string]`

Possible Values: `appCustomProductPage, appCustomProductPageLocalizations`

`limit[appCustomProductPageLocalizations]`

`integer`

Maximum: `50`

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/c7eadc0b-48d9-48c4-bdb2-109dd94a793a
```

```
{
  "data": {
    "type": "appCustomProductPageVersions",
    "id": "c7eadc0b-48d9-48c4-bdb2-109dd94a793a",
    "attributes": {
      "version": "1",
      "state": "PREPARE_FOR_SUBMISSION"
    },
    "relationships": {
      "appCustomProductPageLocalizations": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/c7eadc0b-48d9-48c4-bdb2-109dd94a793a/relationships/appCustomProductPageLocalizations",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/c7eadc0b-48d9-48c4-bdb2-109dd94a793a/appCustomProductPageLocalizations"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/c7eadc0b-48d9-48c4-bdb2-109dd94a793a"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions/c7eadc0b-48d9-48c4-bdb2-109dd94a793a"
  }
}
```

## See Also

### Endpoints

List custom product page versions

List the versions for a custom product page version.

List custom product pages localizations

List all localizations for an app custom product page.

Create a custom product page version

Add a version for your app custom product page.

Modify a custom product page version

Update the name and visibility status of an app custom product page.

