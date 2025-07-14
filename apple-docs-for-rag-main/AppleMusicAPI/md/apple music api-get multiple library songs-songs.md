

- Apple Music API
-  Get Multiple Library Songs 

Web Service Endpoint

# Get Multiple Library Songs

Fetch one or more library songs by using their identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/songs
```

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the library songs. The maximum fetch limit is 300. For possible values, get all the library songs by sending this endpoint without the `ids` parameter.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`include`

`[string]`

Additional relationships to include in the fetch.

`extend`

`[string]`

A response indicating an error occurred on the server.

## Response Codes

` 200 ``OK`

LibrarySongsResponse

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
https://api.music.apple.com/v1/me/library/songs?ids=i.PkdJNdAIrQozOW
```

```
{    
    "data": [
        {
            "id": "i.PkdJNdAIrQozOW",
            "type": "library-songs",
            "href": "/v1/me/library/songs/i.PkdJNdAIrQozOW",
            "attributes": {
                "discNumber": 1,
                "albumName": "Un Verano Sin Ti",
                "genreNames": [
                    "Latin"
                ],
                "trackNumber": 10,
                "hasLyrics": true,
                "releaseDate": "2022-05-06",
                "durationInMillis": 213061,
                "name": "Efecto",
                "artistName": "Bad Bunny",
                "artwork": {
                    "width": 1200,
                    "height": 1200,
                    "url": "https://is5-ssl.mzstatic.com/image/thumb/Music112/v4/3e/04/eb/3e04ebf6-370f-f59d-ec84-2c2643db92f1/196626945068.jpg/{w}x{h}bb.jpg"
                },
                "playParams": {
                    "id": "i.PkdJNdAIrQozOW",
                    "kind": "song",
                    "isLibrary": true,
                    "reporting": true,
                    "catalogId": "1622045954",
                    "reportingId": "1622045954"
                }
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

Get a Library Song's Relationship Directly by Name

Fetch a library song’s relationship by using its identifier.

Get All Library Songs

Fetch all the library songs in alphabetical order.

