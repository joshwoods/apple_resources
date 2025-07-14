

- Apple Music API
-  Create a New Library Playlist Folder 

Web Service Endpoint

# Create a New Library Playlist Folder

Create a new playlist folder in a user’s library.

Apple Music 1.0+

## URL

``` source
POST https://api.music.apple.com/v1/me/library/playlist-folders
```

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## HTTP Body

LibraryPlaylistFolderCreationRequest

The `POST` request containing the `name` and `parent` playlist folder for the playlist folder to be added.

Content-Type: application/json

## Response Codes

` 201 ``Created`

LibraryPlaylistFoldersResponse

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

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/library/playlist-folders
```

```
{
    "data": [
        {
            "id": "p.WmzVVDOUO9pDBk",
            "type": "library-playlist-folders",
            "href": "/v1/me/library/playlist-folders/p.WmzVVDOUO9pDBk",
            "attributes": {
                "name": "Chill",
                "dateAdded": "2022-03-19T06:07:33Z"
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

object LibraryPlaylists

A resource object that represents a library playlist.

object LibraryPlaylistsResponse

The response to a library playlists request.

### Handling Library Playlist Folders

Get Root Library Playlists Folder

Fetch the root library playlists folder for the user.

Get a Library Playlist Folder

Fetch a library playlist folder by using its identifier.

Get a Library Playlist Folder’s Relationship Directly by Name

Fetch a library playlist folder’s relationship by using its identifier.

Get Multiple Library Playlist Folders

Fetch one or more library playlist folders by using their identifiers.

object LibraryPlaylistFolderCreationRequest

Request object to create a new library playlist folder.

