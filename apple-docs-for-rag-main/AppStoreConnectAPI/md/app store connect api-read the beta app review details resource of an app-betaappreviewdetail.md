

- App Store Connect API
-  Read the Beta App Review Details Resource of an App 

Web Service Endpoint

# Read the Beta App Review Details Resource of an App

Get the beta app review details for a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/betaAppReviewDetail
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[betaAppReviewDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, app`

## Response Codes

` 200 ``OK`

BetaAppReviewDetailWithoutIncludesResponse

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
https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppReviewDetail
```

```
{
    "data": {
        "type": "betaAppReviewDetails",
        "id": "6446998023",
        "attributes": {
            "contactFirstName": "Johnny",
            "contactLastName": "Appleseed",
            "contactPhone": "8001234567",
            "contactEmail": "example@apple.com",
            "demoAccountName": null,
            "demoAccountPassword": null,
            "demoAccountRequired": false,
            "notes": null
        },
        "relationships": {
            "app": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/betaAppReviewDetails/6446998023/relationships/app",
                    "related": "https://api.appstoreconnect.apple.com/v1/betaAppReviewDetails/6446998023/app"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/betaAppReviewDetails/6446998023"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppReviewDetail"
    }
}

```

## See Also

### Getting an app’s TestFlight details

Read the Beta License Agreement of an App

Get the beta license agreement for a specific app.

List All Beta App Localizations of an App

Get a list of localized beta test information for a specific app.

