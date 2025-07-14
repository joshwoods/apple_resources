

- App Store Connect API
-  Read the Beta License Agreement of an App 

Web Service Endpoint

# Read the Beta License Agreement of an App

Get the beta license agreement for a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/betaLicenseAgreement
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[betaLicenseAgreements]`

`[string]`

Fields to return for included related types.

Possible Values: `agreementText, app`

## Response Codes

` 200 ``OK`

BetaLicenseAgreementWithoutIncludesResponse

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
https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaLicenseAgreement
```

```
{
    "data": {
        "type": "betaLicenseAgreements",
        "id": "66237ae8-4920-497d-90f5-3f9acc76ec95",
        "attributes": {
            "agreementText": "This is the Beta License Agreement for your Your Next Cortado. You are testing pre-release version of this app. Here are some more thoughts about a beta coffee app. The coffee might not be dialed in and you may experience less than perfect coffee."
        },
        "relationships": {
            "app": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/betaLicenseAgreements/66237ae8-4920-497d-90f5-3f9acc76ec95/relationships/app",
                    "related": "https://api.appstoreconnect.apple.com/v1/betaLicenseAgreements/66237ae8-4920-497d-90f5-3f9acc76ec95/app"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/betaLicenseAgreements/66237ae8-4920-497d-90f5-3f9acc76ec95"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaLicenseAgreement"
    }
}
```

## See Also

### Getting an app’s TestFlight details

Read the Beta App Review Details Resource of an App

Get the beta app review details for a specific app.

List All Beta App Localizations of an App

Get a list of localized beta test information for a specific app.

