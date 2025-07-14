

- Apple Music API
-  Get a Library Song's Relationship Directly by Name 

Web Service Endpoint

# Get a Library Song's Relationship Directly by Name

Fetch a library song’s relationship by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/songs/{id}/{relationship}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the library song.

`relationship`

`string`

 (Required) 

The name of the relationship you want to fetch for this resource.

Possible Values: `albums, artists, catalog`

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`include`

`[string]`

Additional relationships to include in the fetch.

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

Default: `25`

Maximum: `100`

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

RelationshipResponse

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains the requested resource object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/library/songs/i.PkdJNdAIrQozOW/albums
```

```
{    
    "data": [
        {
            "id": "l.fsnYeFy",
            "type": "library-albums",
            "href": "/v1/me/library/albums/l.fsnYeFy",
            "attributes": {
                "trackCount": 1,
                "genreNames": [
                    "Latin"
                ],
                "releaseDate": "2022-05-06",
                "name": "Un Verano Sin Ti",
                "artistName": "Bad Bunny",
                "artwork": {
                    "width": 1200,
                    "height": 1200,
                    "url": "https://is5-ssl.mzstatic.com/image/thumb/Music112/v4/3e/04/eb/3e04ebf6-370f-f59d-ec84-2c2643db92f1/196626945068.jpg/{w}x{h}bb.jpg"
                },
                "playParams": {
                    "id": "l.fsnYeFy",
                    "kind": "album",
                    "isLibrary": true
                },
                "dateAdded": "2022-08-06T02:51:42Z"
            }
        }
    ]
}
```

## See Also

### Related Documentation

object LibrarySongs

A resource object that represents a library song.

object LibrarySongsResponse

The response to a library songs request.

### Requesting a Library Song

Get a Library Song

Fetch a library song by using its identifier.

Get Multiple Library Songs

Fetch one or more library songs by using their identifiers.

Get All Library Songs

Fetch all the library songs in alphabetical order.

