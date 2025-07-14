

- Apple Music API
-  Get a Catalog Curator 

Web Service Endpoint

# Get a Catalog Curator

Fetch a curator by using the curator’s identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/curators/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the curator.

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

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

CuratorsResponse

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains a single `Curator` object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/curators/1107687517
```

```
{
    "data": [
        {
            "attributes": {
                "artwork": {
                    "bgColor": "ffffff",
                    "height": 1080,
                    "textColor1": "000000",
                    "textColor2": "2d2d2d",
                    "textColor3": "333333",
                    "textColor4": "575757",
                    "url": "https://example.mzstatic.com/image/thumb/Features30/v4/8a/d7/80/8ad7800c-06cd-db72-91c7-55ff8bec0346/source/{w}x{h}bb.jpeg",
                    "width": 1080
                },
                "editorialNotes": {
                    "short": "LargeUp is the global platform for Caribbean music, arts and culture. ",
                    "standard": "LargeUp, the global platform for Caribbean music, arts and culture. Since 2009, LargeUp.com has captured the vibrant sounds, styles, flavors, destinations and activities of the islands, spotlighting the best in reggae, dancehall, soca, reggaeton and kompa."
                },
                "name": "LargeUp",
                "url": "https://itunes.apple.com/us/curator/largeup/id1107687517"
            },
            "href": "/v1/catalog/us/curators/1107687517",
            "id": "1107687517",
            "relationships": {
                "playlists": {
                    "data": [],
                    "href": "/v1/catalog/us/curators/1107687517/playlists"
                }
            },
            "type": "curators"
        }
    ]
}
```

## See Also

### Related Documentation

object Curators

A resource object that represents a curator.

object CuratorsResponse

The response to a request for curators.

### Requesting Catalog Curators

Get a Catalog Curator's Relationship Directly by Name

Fetch a curator’s relationship by using its identifier.

Get Multiple Catalog Curators

Fetch one or more curators by using their identifiers.

