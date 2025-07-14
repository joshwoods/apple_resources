

- Apple Music API
-  Get Multiple Personal Album Ratings 

Web Service Endpoint

# Get Multiple Personal Album Ratings

Fetch the user’s ratings for one or more albums by using the albums’ identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/ratings/albums
```

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the albums.

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

RatingsResponse

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

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

A rating indicates whether a user likes `(1)` or dislikes `(-1)` the album. These are the only two ratings supported.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/ratings/albums?ids=1138988512,475655712
```

```
{
    "data": [
        {
            "attributes": {
                "value": 1
            },
            "href": "/v1/me/ratings/albums/1138988512",
            "id": "1138988512",
            "type": "ratings"
        },
        {
            "attributes": {
                "value": 1
            },
            "href": "/v1/me/ratings/albums/475655712",
            "id": "475655712",
            "type": "ratings"
        }
    ]
}
```

## See Also

### Related Documentation

object Ratings

An object that represents a rating for a resource.

object RatingRequest

A request containing the data for a rating.

object RatingsResponse

The response to a request for a rating.

### Requesting Catalog Ratings

Get a Personal Album Rating

Fetch a user’s rating for an album by using the user’s identifier.

Get a Personal Music Video Rating

Fetch a user’s rating for a music video by using the video’s identifier.

Get a Personal Playlist Rating

Fetch a user’s rating for a playlist by using the playlist’s identifier.

Get a Personal Song Rating

Fetch a user’s rating for a song by using the song’s identifier.

Get a Personal Station Rating

Fetch a user’s rating for a station by using the station’s identifier.

Get Multiple Personal Music Video Ratings

Fetch the user’s ratings for one or more music videos by using the music videos’ identifiers.

Get Multiple Personal Playlist Ratings

Fetch the user’s ratings for one or more playlists by using the playlists’ identifiers.

Get Multiple Personal Song Ratings

Fetch the user’s ratings for one or more songs by using the songs’ identifiers.

Get Multiple Personal Station Ratings

Fetch the user’s ratings for one or more stations by using the stations’ identifiers.

