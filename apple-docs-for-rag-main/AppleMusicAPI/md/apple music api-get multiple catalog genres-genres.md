

- Apple Music API
-  Get Multiple Catalog Genres 

Web Service Endpoint

# Get Multiple Catalog Genres

Fetch one or more genres for a specific storefront.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/genres
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the catalog genres. For possible values, get all the genres for the current top charts by sending this endpoint without the `ids` parameter.

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

GenresResponse

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains an array of `Genre` objects. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/genres?ids=14,21
```

```
{
    "data": [
        {
            "attributes": {
                "name": "Pop"
            },
            "href": "/v1/catalog/us/genres/14",
            "id": "14",
            "type": "genres"
        },
        {
            "attributes": {
                "name": "Rock"
            },
            "href": "/v1/catalog/us/genres/21",
            "id": "21",
            "type": "genres"
        }
    ]
}
```

## See Also

### Related Documentation

object Genres

A resource object that represents a music genre.

object GenresResponse

The response to a genres request.

### Requesting Catalog Genres

Get a Catalog Genre

Fetch a genre by using its identifier.

Get Catalog Top Charts Genres

Fetch all genres for the current top charts.

