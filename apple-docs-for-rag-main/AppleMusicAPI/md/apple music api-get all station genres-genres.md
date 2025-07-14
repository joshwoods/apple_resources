

- Apple Music API
-  Get All Station Genres 

Web Service Endpoint

# Get All Station Genres

Fetch all station genres for a given storefront.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/station-genres
```

## Path Parameters

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

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

`offset`

`string`

The offset to use for a paginated request.

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
https://api.music.apple.com/v1/catalog/us/station-genres
```

```
{
    "data": [
        {
            "id": "1149486245",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486245",
            "attributes": {
                "name": "Electronic"
            }
        },
        {
            "id": "1149486314",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486314",
            "attributes": {
                "name": "Latin"
            }
        },
        {
            "id": "1149486325",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486325",
            "attributes": {
                "name": "Metal"
            }
        },
        {
            "id": "1149486238",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486238",
            "attributes": {
                "name": "Dance"
            }
        },
        {
            "id": "1149486299",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486299",
            "attributes": {
                "name": "Jazz"
            }
        },
        {
            "id": "1149486336",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486336",
            "attributes": {
                "name": "Pop"
            }
        },
        {
            "id": "1149486287",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486287",
            "attributes": {
                "name": "Hip-Hop/R&B"
            }
        },
        {
            "id": "1149486381",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486381",
            "attributes": {
                "name": "Workout"
            }
        },
        {
            "id": "1149486231",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486231",
            "attributes": {
                "name": "Country"
            }
        },
        {
            "id": "1184713285",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1184713285",
            "attributes": {
                "name": "Holiday"
            }
        },
        {
            "id": "1149484144",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149484144",
            "attributes": {
                "name": "Alternative & Indie"
            }
        },
        {
            "id": "1149486361",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486361",
            "attributes": {
                "name": "Reggae"
            }
        },
        {
            "id": "1149486377",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486377",
            "attributes": {
                "name": "Singer/Songwriter"
            }
        },
        {
            "id": "1149486281",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486281",
            "attributes": {
                "name": "From Around the World"
            }
        },
        {
            "id": "1149486223",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486223",
            "attributes": {
                "name": "Christian"
            }
        },
        {
            "id": "1154291546",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1154291546",
            "attributes": {
                "name": "Hits by Decade"
            }
        },
        {
            "id": "1149486227",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486227",
            "attributes": {
                "name": "Classical"
            }
        },
        {
            "id": "1149486306",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486306",
            "attributes": {
                "name": "Kids & Family"
            }
        },
        {
            "id": "1149486365",
            "type": "station-genres",
            "href": "/v1/catalog/us/station-genres/1149486365",
            "attributes": {
                "name": "Rock"
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

Get a Station Genre

Fetch a station genre by using its identifier.

Get a Station Genre’s Relationship Directly by Name

Fetch a station genre’s relationship by using its identifier.

Get Multiple Stations Genres

Fetch one or more station genres by using their identifiers.

