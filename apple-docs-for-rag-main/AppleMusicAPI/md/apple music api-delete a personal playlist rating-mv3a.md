

- Apple Music API
-  Delete a Personal Playlist Rating 

Web Service Endpoint

# Delete a Personal Playlist Rating

Remove a user’s playlist rating by using the playlist’s identifier.

Apple Music 1.0+

## URL

``` source
DELETE https://api.music.apple.com/v1/me/ratings/playlists/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the playlist.

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## Response Codes

` 204 ``No Content`

EmptyBodyResponse

`No Content`

The modification was successful, but there’s no content in the response.

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

A rating indicates whether a user likes `(1)` or dislikes `(-1)` the playlist. These are the only two ratings supported.

For a particular playlist, the personal ratings for that playlist’s catalog ID and library ID (if the playlist is in the library) stay synced.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/ratings/playlists/pl.5b0194eaa170401e8986335d7e77aa4e
```

```
No response body.
```

## See Also

### Related Documentation

object Ratings

An object that represents a rating for a resource.

### Deleting Catalog Ratings

Delete a Personal Album Rating

Remove a user’s album rating by using the album’s identifier.

Delete a Personal Music Video Rating

Remove a user’s music video rating by using the music video’s identifier.

Delete a Personal Song Rating

Remove a user’s song rating by using the song’s identifier.

Delete a Personal Station Rating

Remove a user’s station rating by using the station’s identifier.

