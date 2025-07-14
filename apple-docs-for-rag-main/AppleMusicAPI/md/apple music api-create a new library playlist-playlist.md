

- Apple Music API
-  Create a New Library Playlist 

Web Service Endpoint

# Create a New Library Playlist

Create a new playlist in a user’s library.

Apple Music 1.0+

## URL

``` source
POST https://api.music.apple.com/v1/me/library/playlists
```

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## HTTP Body

LibraryPlaylistCreationRequest

The `POST` request containing the `name`**,** `tracks` and `parent` playlist folder for the playlist to be added.

Content-Type: application/json

## Response Codes

` 201 ``Created`

LibraryPlaylistsResponse

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
https://api.music.apple.com/v1/me/library/playlists
```

```
{    "data": [
        {
            "id": "p.RB1AAkGsv74Zkl",
            "type": "library-playlists",
            "href": "/v1/me/library/playlists/p.RB1AAkGsv74Zkl",
            "attributes": {
                "hasCatalog": false,
                "description": {
                    "standard": "My library playlist"
                },
                "name": "New Playlist",
                "canEdit": true,
                "isPublic": false,
                "playParams": {
                    "id": "p.RB1AAkGsv74Zkl",
                    "kind": "playlist",
                    "isLibrary": true
                },
                "dateAdded": "2021-09-30T13: 28: 29Z"
            }
        }
    ]
}
```

## See Also

### Related Documentation

object LibraryPlaylists

A resource object that represents a library playlist.

object LibraryPlaylistsResponse

The response to a library playlists request.

### Creating and Modifying User Playlists

Add Tracks to a Library Playlist

Add new tracks to the end of a library playlist.

Add a Resource to a Library

Add a catalog resource to a user’s iCloud Music Library.

object LibraryPlaylistCreationRequest

A request to create a new playlist in a user’s library.

object LibraryPlaylistTracksRequest

A request to add tracks to a library playlist.

