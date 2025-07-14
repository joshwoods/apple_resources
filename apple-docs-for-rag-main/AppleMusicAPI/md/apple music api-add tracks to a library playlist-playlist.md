

- Apple Music API
-  Add Tracks to a Library Playlist 

Web Service Endpoint

# Add Tracks to a Library Playlist

Add new tracks to the end of a library playlist.

Apple Music 1.0+

## URL

``` source
POST https://api.music.apple.com/v1/me/library/playlists/{id}/tracks
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier of the library playlist.

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## HTTP Body

LibraryPlaylistTracksRequest

The `POST` request containing the `identifier` and `type` for the tracks to be added.

Content-Type: application/json

## Response Codes

` 201 ``Created`

LibraryPlaylistsTracksRelationshipResponse

`Created`

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

If successful, the HTTP status code is 201 (Created) and a new resource created as a result. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

Note

There may be a delay before a new resource appears in a user’s library.

You can include an optional `tracks` relationship in this request.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/library/playlists/p.RB1AARBIv74Zkl/tracks
```

```
No response body
```

## See Also

### Related Documentation

object LibraryPlaylists

A resource object that represents a library playlist.

object LibraryPlaylistsResponse

The response to a library playlists request.

### Creating and Modifying User Playlists

Create a New Library Playlist

Create a new playlist in a user’s library.

Add a Resource to a Library

Add a catalog resource to a user’s iCloud Music Library.

object LibraryPlaylistCreationRequest

A request to create a new playlist in a user’s library.

object LibraryPlaylistTracksRequest

A request to add tracks to a library playlist.

