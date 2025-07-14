

- Apple Music API
-  Get Catalog Search Hints 

Web Service Endpoint

# Get Catalog Search Hints

Fetch the search term results for a hint.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/search/hints
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`term`

`string`

 (Required) 

The entered text for the search with ‘`+`’ characters between each word, to replace spaces (for example `term=james+br`).

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

Default: `10`

## Response Codes

` 200 ``OK`

SearchHintsResponse

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

If successful, the HTTP status code is 200 (OK) and the `results` object contains a single `terms` array. This array contains a list of possible valid search queries determined from the search hint. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

These results are autocompletion options for the hint and are potential search terms. For more information, see Search for Catalog Resources.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/search/hints?term=beach+bunny
```

```
{
    "results": {
        "terms": [
            "beach bunny",
            "oxygen beach bunny",
            "cloud 9 beach bunny"
        ]
    }
}
```

## See Also

### Related Documentation

object SearchHintsResponse

The response to a request for search hints.

### Searching for Catalog Resources

Search for Catalog Resources

Search the catalog by using a query.

Get Catalog Search Suggestions

Fetch the search suggestions for a provided term input.

