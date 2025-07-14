

- Apple Music API
-  Get a User's Storefront 

Web Service Endpoint

# Get a User's Storefront

Fetch a storefront for a specific user.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/storefront
```

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

`include`

`[string]`

Additional relationships to include in the fetch.

`offset`

`string`

The offset to use for a paginated request. See Fetching Resources by Page.

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

PaginatedResourceCollectionResponse

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

A response indicating an incorrect `Authorization` header.

Content-Type: application/json

` 403 ``Forbidden`

ForbiddenResponse

`Forbidden`

A response indicating invalid or insufficient authentication.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

A response indicating an error occurred on the server.

Content-Type: application/json

## Discussion

If successful, the HTTP status code is 200 (OK) and the `data` array contains a single Storefronts object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/storefront
```

```
{
    "data": [
        {
            "id": "us",
            "type": "storefronts",
            "href": "/v1/storefronts/us",
            "attributes": {
                "supportedLanguageTags": [
                    "en-US",
                    "es-MX",
                    "ar",
                    "ru",
                    "zh-Hans-CN"
                ],
                "defaultLanguageTag": "en-US",
                "name": "United States",
                "explicitContentPolicy": "allowed"
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

