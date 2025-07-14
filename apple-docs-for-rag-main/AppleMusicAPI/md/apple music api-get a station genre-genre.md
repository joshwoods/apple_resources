

- Apple Music API
-  Get a Station Genre 

Web Service Endpoint

# Get a Station Genre

Fetch a station genre by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/station-genres/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the station genre.

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`include`

`[string]`

Additional relationships to include in the fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

StationGenresResponse

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains the requested resource object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/station-genres/1149486336
```

```
{
    "data": [
        {
            "id": "1149486336",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486336",
            "attributes": {
                "name": "Pop"
            }
        }
    ]
}

```

## See Also

### Related Documentation

object StationGenres

A resource object that represents a station genre.

object StationGenresResponse

The response to a specific station genres resource request.

### Requesting a Catalog Station Genre

Get a Station Genre’s Relationship Directly by Name

Fetch a station genre’s relationship by using its identifier.

Get Multiple Stations Genres

Fetch one or more station genres by using their identifiers.

Get All Station Genres

Fetch all station genres for a given storefront.

