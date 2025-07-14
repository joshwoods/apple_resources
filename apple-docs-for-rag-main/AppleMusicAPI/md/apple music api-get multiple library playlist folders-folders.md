

- Apple Music API
-  Get Multiple Library Playlist Folders 

Web Service Endpoint

# Get Multiple Library Playlist Folders

Fetch one or more library playlist folders by using their identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/playlist-folders
```

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the playlist folders.

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

LibraryPlaylistFoldersResponse

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
https://api.music.apple.com/v1/me/library/playlist-folders?ids=p.WmzVVDOUO9pDBk
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
                "dateAdded": "2022-03-19T06: 07: 33Z"
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

### Handling Library Playlist Folders

Get Root Library Playlists Folder

Fetch the root library playlists folder for the user.

Get a Library Playlist Folder

Fetch a library playlist folder by using its identifier.

Get a Library Playlist Folder’s Relationship Directly by Name

Fetch a library playlist folder’s relationship by using its identifier.

Create a New Library Playlist Folder

Create a new playlist folder in a user’s library.

object LibraryPlaylistFolderCreationRequest

Request object to create a new library playlist folder.

