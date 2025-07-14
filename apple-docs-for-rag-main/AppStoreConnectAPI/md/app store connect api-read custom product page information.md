

- App Store Connect API
-  Read custom product page information 

Web Service Endpoint

# Read custom product page information

Get information about a specific app custom product page.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page resource ID from the List all custom product pages for an app response.

## Query Parameters

`fields[appCustomProductPageVersions]`

`[string]`

Possible Values: `version, state, deepLink, appCustomProductPage, appCustomProductPageLocalizations`

`fields[appCustomProductPages]`

`[string]`

Possible Values: `name, url, visible, app, appCustomProductPageVersions`

`include`

`[string]`

Possible Values: `app, appCustomProductPageVersions`

`limit[appCustomProductPageVersions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppCustomProductPageResponse

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
https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3
```

```
{
  "data": {
    "type": "appCustomProductPages",
    "id": "eb2b3606-2fef-4aab-a54e-b2e5547c9bc3",
    "attributes": {
      "name": "Custom Product Page May 1",
      "url": "https://apps.apple.com/us/app/gersey-numba/id1526908970?ppid=eb2b3606-2fef-4aab-a54e-b2e5547c9bc3",
      "visible": false
    },
    "relationships": {
      "appCustomProductPageVersions": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3/relationships/appCustomProductPageVersions",
          "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3/appCustomProductPageVersions"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3"
  }
}
```

## See Also

### Endpoints

Create a custom product page

Add a custom product page for your app.

Modify an app custom product page

Update the name and visibility status of an app custom product page.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

List custom product page versions

List the versions for a custom product page version.

Delete an app custom product page

Delete metadata that you configured for a custom product page.

