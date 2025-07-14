

- App Store Connect API
-  Read the End User License Agreement Information of an App 

Web Service Endpoint

# Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/endUserLicenseAgreement
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[endUserLicenseAgreements]`

`[string]`

Possible Values: `agreementText, app, territories`

## Response Codes

` 200 ``OK`

EndUserLicenseAgreementWithoutIncludesResponse

`OK`

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/1000001234/endUserLicenseAgreement
```

```
{
  "data": {
    "type": "endUserLicenseAgreements",
    "id": "d187a413-70fb-45c7-ae43-12345ea0d40",
    "attributes": {
      "agreementText": "This is the agreement. It is vital you read it."
    },
    "relationships": {
      "territories": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/d187a413-70fb-45c7-ae43-12345ea0d40/relationships/territories",
          "related": "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/d187a413-70fb-45c7-ae43-12345ea0d40/territories"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/d187a413-70fb-45c7-ae43-12345ea0d40"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/1000001234/endUserLicenseAgreement"
  }
}
```

## See Also

### Getting App Store details for your app

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

GET /v1/apps/{id}/appStoreVersionExperimentsV2

