

- Apple Music API
-  Search for Library Resources 

Web Service Endpoint

# Search for Library Resources

Search the library by using a query.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/search
```

## Query Parameters

`term`

`string`

 (Required) 

The text for the search, with a plus sign (`+`) between each word to replace spaces (for example, `term=james+br`).

`types`

`[string]`

 (Required) 

The list of the types of resources to include in the results. The possible values are `library-albums`, `library-songs`, `library-playlists`, `library-artists`, and `library-music-videos`.

Possible Values: `library-albums, library-artists, library-music-videos, library-playlists, library-songs`

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

Default: `5`

Maximum: `25`

`offset`

`string`

The next page or group of objects to fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## Response Codes

` 200 ``OK`

LibrarySearchResponse

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

If successful, the HTTP status code is 200 (OK) and the `results` contains a map of search results. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/library/search?types=library-songs,library-albums&term=Happier
```

```
{
    "results": {
        "library-songs": {
            "href": "/v1/me/library/search?term=Happier&types=library-songs",
            "next": "/v1/me/library/search?offset=5&term=Happier&types=library-songs",
            "data": [
                {
                    "id": "i.PkdNMlmi2og2p5",
                    "type": "library-songs",
                    "href": "/v1/me/library/songs/i.PkdNMlmi2og2p5",
                    "attributes": {
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        },
                        "artistName": "Billie Eilish",
                        "discNumber": 1,
                        "genreNames": [
                            "Alternative"
                        ],
                        "durationInMillis": 206623,
                        "releaseDate": "2021-07-30",
                        "name": "Everybody Dies",
                        "hasLyrics": true,
                        "albumName": "Happier Than Ever",
                        "playParams": {
                            "id": "i.PkdNMlmi2og2p5",
                            "kind": "song",
                            "isLibrary": true,
                            "reporting": true,
                            "catalogId": "1564530960"
                        },
                        "trackNumber": 11
                    }
                },
                {
                    "id": "i.gelNOLouL41Lxo",
                    "type": "library-songs",
                    "href": "/v1/me/library/songs/i.gelNOLouL41Lxo",
                    "attributes": {
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        },
                        "artistName": "Billie Eilish",
                        "discNumber": 1,
                        "genreNames": [
                            "Alternative"
                        ],
                        "durationInMillis": 214059,
                        "releaseDate": "2021-07-30",
                        "name": "OverHeated",
                        "hasLyrics": true,
                        "albumName": "Happier Than Ever",
                        "playParams": {
                            "id": "i.gelNOLouL41Lxo",
                            "kind": "song",
                            "isLibrary": true,
                            "reporting": true,
                            "catalogId": "1564530959"
                        },
                        "trackNumber": 10,
                        "contentRating": "explicit"
                    }
                },
                {
                    "id": "i.1YBx1GAHq0vqZP",
                    "type": "library-songs",
                    "href": "/v1/me/library/songs/i.1YBx1GAHq0vqZP",
                    "attributes": {
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        },
                        "artistName": "Billie Eilish",
                        "discNumber": 1,
                        "genreNames": [
                            "Alternative"
                        ],
                        "durationInMillis": 195777,
                        "releaseDate": "2021-06-09",
                        "name": "NDA",
                        "hasLyrics": true,
                        "albumName": "Happier Than Ever",
                        "playParams": {
                            "id": "i.1YBx1GAHq0vqZP",
                            "kind": "song",
                            "isLibrary": true,
                            "reporting": true,
                            "catalogId": "1564531177"
                        },
                        "trackNumber": 13,
                        "contentRating": "explicit"
                    }
                },
                {
                    "id": "i.QvzN9lPfVx2VZ3",
                    "type": "library-songs",
                    "href": "/v1/me/library/songs/i.QvzN9lPfVx2VZ3",
                    "attributes": {
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        },
                        "artistName": "Billie Eilish",
                        "discNumber": 1,
                        "genreNames": [
                            "Alternative"
                        ],
                        "durationInMillis": 196731,
                        "releaseDate": "2021-07-30",
                        "name": "Billie Bossa Nova",
                        "hasLyrics": true,
                        "albumName": "Happier Than Ever",
                        "playParams": {
                            "id": "i.QvzN9lPfVx2VZ3",
                            "kind": "song",
                            "isLibrary": true,
                            "reporting": true,
                            "catalogId": "1564530941"
                        },
                        "trackNumber": 3
                    }
                },
                {
                    "id": "i.gelNOzPuL41Lxo",
                    "type": "library-songs",
                    "href": "/v1/me/library/songs/i.gelNOzPuL41Lxo",
                    "attributes": {
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        },
                        "artistName": "Billie Eilish",
                        "discNumber": 1,
                        "genreNames": [
                            "Alternative"
                        ],
                        "durationInMillis": 298899,
                        "releaseDate": "2021-07-30",
                        "name": "Happier Than Ever",
                        "hasLyrics": true,
                        "albumName": "Happier Than Ever",
                        "playParams": {
                            "id": "i.gelNOzPuL41Lxo",
                            "kind": "song",
                            "isLibrary": true,
                            "reporting": true,
                            "catalogId": "1564531202"
                        },
                        "trackNumber": 15,
                        "contentRating": "explicit"
                    }
                }
            ]
        },
        "library-albums": {
            "href": "/v1/me/library/search?term=Happier&types=library-albums",
            "data": [
                {
                    "id": "l.qrRWYhq",
                    "type": "library-albums",
                    "href": "/v1/me/library/albums/l.qrRWYhq",
                    "attributes": {
                        "playParams": {
                            "id": "l.qrRWYhq",
                            "kind": "album",
                            "isLibrary": true
                        },
                        "dateAdded": "2021-09-10T18: 12: 57Z",
                        "artistName": "Billie Eilish",
                        "trackCount": 16,
                        "name": "Happier Than Ever",
                        "genreNames": [
                            "Alternative"
                        ],
                        "releaseDate": "2021-07-30",
                        "artwork": {
                            "width": 1200,
                            "height": 1200,
                            "url": "https: //is3-ssl.mzstatic.com/image/thumb/Music115/v4/2d/f3/c9/2df3c9fd-e0eb-257c-c035-b04f05a66580/21UMGIM36691.rgb.jpg/{w}x{h}bb.jpeg"
                        }
                    }
                }
            ]
        }
    },
    "meta": {
        "results": {
            "order": [
                "library-songs",
                "library-albums"
            ]
        }
    }
}

```

## See Also

### Related Documentation

object LibrarySearchResponse

The response to a request for a library search.

