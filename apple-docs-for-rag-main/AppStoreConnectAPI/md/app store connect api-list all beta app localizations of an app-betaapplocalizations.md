

- App Store Connect API
-  List All Beta App Localizations of an App 

Web Service Endpoint

# List All Beta App Localizations of an App

Get a list of localized beta test information for a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/betaAppLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[betaAppLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `feedbackEmail, marketingUrl, privacyPolicyUrl, tvOsPrivacyPolicy, description, locale, app`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaAppLocalizationsWithoutIncludesResponse

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
https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppLocalizations
```

```
{
    "data": [
        {
            "type": "betaAppLocalizations",
            "id": "318d7ad7-6d08-403d-84f4-1eb8d9ba9071",
            "attributes": {
                "feedbackEmail": "example@apple.com",
                "marketingUrl": null,
                "privacyPolicyUrl": null,
                "tvOsPrivacyPolicy": null,
                "description": null,
                "locale": "en-US"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/betaAppLocalizations/318d7ad7-6d08-403d-84f4-1eb8d9ba9071/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/betaAppLocalizations/318d7ad7-6d08-403d-84f4-1eb8d9ba9071/app"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/betaAppLocalizations/318d7ad7-6d08-403d-84f4-1eb8d9ba9071"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppLocalizations"
    },
    "meta": {
        "paging": {
            "total": 1,
            "limit": 50
        }
    }
}
```

## See Also

### Getting an app’s TestFlight details

Read the Beta App Review Details Resource of an App

Get the beta app review details for a specific app.

Read the Beta License Agreement of an App

Get the beta license agreement for a specific app.

