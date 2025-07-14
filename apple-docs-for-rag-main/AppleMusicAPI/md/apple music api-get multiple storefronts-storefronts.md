

- Apple Music API
-  Get Multiple Storefronts 

Web Service Endpoint

# Get Multiple Storefronts

Fetch one or more storefronts by using their identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/storefronts
```

## Query Parameters

`ids`

`[string]`

 (Required) 

A list of the identifiers (ISO 3166 alpha-2 country codes) for the storefronts you want to fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`include`

`[string]`

Additional relationships to include in the fetch.

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

StorefrontsResponse

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

A response indicating an incorrect `Authorization` header.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

A response indicating an error occurred on the server.

Content-Type: application/json

## Discussion

If successful, the HTTP status code is 200 (OK) and the `data` array contains one or more Storefronts objects. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/storefronts?ids=us,ca,cn,au,hk
```

```
{
    "data": [
        {
            "id": "us",
            "type": "storefronts",
            "href": "/v1/storefronts/us",
            "attributes": {
                "explicitContentPolicy": "allowed",
                "defaultLanguageTag": "en-US",
                "name": "United States",
                "supportedLanguageTags": [
                    "en-US",
                    "es-MX",
                    "ar",
                    "ru",
                    "zh-Hans-CN"
                ]
            }
        },
        {
            "id": "ca",
            "type": "storefronts",
            "href": "/v1/storefronts/ca",
            "attributes": {
                "explicitContentPolicy": "allowed",
                "defaultLanguageTag": "en-CA",
                "name": "Canada",
                "supportedLanguageTags": [
                    "en-CA",
                    "fr-CA"
                ]
            }
        },
        {
            "id": "cn",
            "type": "storefronts",
            "href": "/v1/storefronts/cn",
            "attributes": {
                "explicitContentPolicy": "allowed",
                "defaultLanguageTag": "zh-Hans-CN",
                "name": "China mainland",
                "supportedLanguageTags": [
                    "zh-Hans-CN",
                    "en-GB"
                ]
            }
        },
        {
            "id": "au",
            "type": "storefronts",
            "href": "/v1/storefronts/au",
            "attributes": {
                "explicitContentPolicy": "allowed",
                "defaultLanguageTag": "en-AU",
                "name": "Australia",
                "supportedLanguageTags": [
                    "en-AU",
                    "en-GB"
                ]
            }
        },
        {
            "id": "hk",
            "type": "storefronts",
            "href": "/v1/storefronts/hk",
            "attributes": {
                "explicitContentPolicy": "allowed",
                "defaultLanguageTag": "zh-Hant-HK",
                "name": "Hong Kong",
                "supportedLanguageTags": [
                    "zh-Hant-HK",
                    "en-GB",
                    "zh-Hant-TW"
                ]
            }
        }
    ]
}

```

## See Also

### Related Documentation

object Storefronts

A resource object that represents a storefront, an Apple Music and iTunes Store territory that the content is available in.

object StorefrontsResponse

The response to a storefront request.

### Requesting a Catalog Storefront

Get a Storefront

Fetch a single storefront by using its identifier.

Get All Storefronts

Fetch all the storefronts in alphabetical order.

