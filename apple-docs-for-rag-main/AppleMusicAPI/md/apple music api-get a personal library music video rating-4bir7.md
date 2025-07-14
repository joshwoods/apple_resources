

- Apple Music API
-  Get a Personal Library Music Video Rating 

Web Service Endpoint

# Get a Personal Library Music Video Rating

Fetch a user’s rating for a library music video by using the music video’s library identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/ratings/library-music-videos/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the library music video.

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

A rating indicates whether a user likes `(1)` or dislikes `(-1)` the music video. These are the only two ratings supported.

For a particular music video, the personal ratings for that video’s catalog ID and library ID (if the video is in the library) stay synced.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/ratings/library-albums/l.qrRWYhq
```

```
{
    "data": [
        {
            "id": "l.qrRWYhq",
            "type": "ratings",
            "href": "/v1/me/ratings/library-albums/l.qrRWYhq",
            "attributes": {
                "value": 1
            }
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

### Requesting Library Ratings

Get a Personal Library Album Rating

Fetch a user’s rating for specific content by using the content’s identifier.

Get a Personal Library Playlist Rating

Fetch a user’s rating for a library playlist by using the playlist’s library identifier.

Get a Personal Library Song Rating

Fetch a user’s rating for a library song by using the song’s library identifier.

Get Multiple Personal Library Album Ratings

Fetch the user’s ratings for one or more pieces of content by using the contents’ identifiers.

Get Multiple Personal Library Music Video Ratings

Fetch the user’s ratings for one or more library music videos by using the library music videos’ identifiers.

Get Multiple Personal Library Playlist Ratings

Fetch the user’s ratings for one or more library playlists by using the library playlists’ identifiers.

Get Multiple Personal Library Songs Ratings

Fetch the user’s ratings for one or more library songs by using the library songs’ identifiers.

