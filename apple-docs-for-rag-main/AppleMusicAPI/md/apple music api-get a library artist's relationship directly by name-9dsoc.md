

- Apple Music API
-  Get a Library Artist's Relationship Directly by Name 

Web Service Endpoint

# Get a Library Artist's Relationship Directly by Name

Fetch a library artist’s relationship by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/artists/{id}/{relationship}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the library artist.

`relationship`

`string`

 (Required) 

The name of the relationship you want to fetch for this resource.

Possible Values: `albums, catalog`

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
https://api.music.apple.com/v1/me/library/artists/r.y8mMT7t/albums
```

```
{
    "data": [
        {
            "id": "l.sticiFl",
            "type": "library-albums",
            "href": "/v1/me/library/albums/l.sticiFl",
            "attributes": {
                "trackCount": 15,
                "genreNames": [
                    "Country"
                ],
                "releaseDate": "2022-02-11",
                "name": "Bronco",
                "artistName": "Orville Peck",
                "artwork": {
                    "width": 1200,
                    "height": 1200,
                    "url": "https://is3-ssl.mzstatic.com/image/thumb/Music116/v4/6d/de/02/6dde02ae-a9fe-f96e-e81f-4f18ad13d2f9/886449873302.jpg/{w}x{h}bb.jpg"
                },
                "dateAdded": "2022-08-06T02:18:57Z",
                "playParams": {
                    "id": "l.sticiFl",
                    "kind": "album",
                    "isLibrary": true
                }
            }
        }
    ],
    "meta": {
        "total": 1
    }
}
```

## See Also

### Related Documentation

object LibraryArtists

A resource object that represents an artist present in a user’s library.

object LibraryArtistsResponse

The response to a library artists request.

### Requesting a Library Artist

Get a Library Artist

Fetch a library artist by using its identifier.

Get Multiple Library Artists

Fetch one or more library artists by using their identifiers.

Get All Library Artists

Fetch all the library artists in alphabetical order.

