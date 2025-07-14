

- Apple Music API
-  Get a Storefront 

Web Service Endpoint

# Get a Storefront

Fetch a single storefront by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/storefronts/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The identifier (an ISO 3166 alpha-2 country code) for the storefront you want to fetch.

## Query Parameters

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains a single Storefronts object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/storefronts/jp
```

```
{
    "data": [
        {
            "id": "jp",
            "type": "storefronts",
            "href": "/v1/storefronts/jp",
            "attributes": {
                "defaultLanguageTag": "ja",
                "name": "Japan",
                "explicitContentPolicy": "allowed",
                "supportedLanguageTags": [
                    "ja",
                    "en-US"
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

Get Multiple Storefronts

Fetch one or more storefronts by using their identifiers.

Get All Storefronts

Fetch all the storefronts in alphabetical order.

