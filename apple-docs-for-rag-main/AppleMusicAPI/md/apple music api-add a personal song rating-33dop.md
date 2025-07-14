

- Apple Music API
-  Add a Personal Song Rating 

Web Service Endpoint

# Add a Personal Song Rating

Add a user’s song rating by using the song’s identifier.

Apple Music 1.0+

## URL

``` source
PUT https://api.music.apple.com/v1/me/ratings/songs/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the song.

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## HTTP Body

RatingRequest

A dictionary that includes the type and attributes of the resource rating.

Content-Type: application/json

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

A rating indicates whether a user likes `(1)` or dislikes `(-1)` the song. These are the only two ratings supported.

For a particular song, the personal ratings for that song’s catalog ID and library ID (if the playlist is in the library) stay synced.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/ratings/songs/907242702

{
    "type":"rating",
    "attributes":{
        "value":1
    }
}
```

```
{
    "data":[
        {
            "id":"907242702",
            "type":"ratings",
            "href":"/v1/me/ratings/songs/907242702",
            "attributes":{
                "value":1
            }
        }
    ]
}
```

## See Also

### Related Documentation

object Ratings

An object that represents a rating for a resource.

object RatingsResponse

The response to a request for a rating.

### Adding Catalog Ratings

Add a Personal Album Rating

Add a user’s album rating by using the album’s identifier.

Add a Personal Music Video Rating

Add a user’s music video rating by using the music video’s identifier.

Add a Personal Playlist Rating

Add a user’s playlist rating by using the playlist’s identifier.

Add a Personal Station Rating

Add a user’s station rating by using the station’s identifier.

