

- Apple Music API
-  Delete a Personal Library Song Rating 

Web Service Endpoint

# Delete a Personal Library Song Rating

Remove a user’s library song rating by using the library song’s identifier.

Apple Music 1.0+

## URL

``` source
DELETE https://api.music.apple.com/v1/me/ratings/library-songs/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the library song.

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

A rating indicates whether a user likes `(1`) or dislikes `(-1)` the song. These are the only two ratings supported.

For a particular song, the personal ratings for that song’s catalog ID and library ID (if the song is in the library) stay synced.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/ratings/library-songs/i.7PJNN4mfXlD68R
```

```
No response body.
```

## See Also

### Related Documentation

object Ratings

An object that represents a rating for a resource.

### Deleting Library Ratings

Delete a Personal Library Album Rating

Remove a user’s content rating by using the content’s identifier.

Delete a Personal Library Music Video Rating

Remove a user’s library music video rating by using the library music video’s identifier.

Delete a Personal Library Playlist Rating

Remove a user’s library playlist rating by using the library playlist’s identifier.

