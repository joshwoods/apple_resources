

- Apple Music API
-  Get a Library Playlist Folder’s Relationship Directly by Name 

Web Service Endpoint

# Get a Library Playlist Folder’s Relationship Directly by Name

Fetch a library playlist folder’s relationship by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/playlist-folders/{id}/{relationship}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the library playlist folder.

`relationship`

`string`

 (Required) 

The name of the relationship you want to fetch for this resource.

Possible Values: `children, parent`

## Query Parameters

`include`

`[string]`

Additional relationships to include in the fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`limit`

`integer`

The number of objects or number of objects in the specified relationship returned.

Default: `25`

Maximum: `100`

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

RelationshipResponse

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
https://api.music.apple.com/v1/me/library/playlist-folders/p.WmzVVDOUO9pDBk/children
```

```
{    
    "data": [
        {
            "id": "p.RB1AA8bCv74Zkl",
            "type": "library-playlists",
            "href": "/v1/me/library/playlists/p.RB1AA8bCv74Zkl",
            "attributes": {
                "description": {
                    "standard": ""
                },
                "dateAdded": "2021-12-03T19: 06: 29Z",
                "hasCatalog": true,
                "isPublic": false,
                "playParams": {
                    "id": "p.RB1AA8bCv74Zkl",
                    "kind": "playlist",
                    "isLibrary": true,
                    "globalId": "pl.u-jV8990gT3bLqrj"
                },
                "name": "Chill JPop",
                "canEdit": true
            }
        },
        {
            "id": "p.eoGxpgbtxAPJG6",
            "type": "library-playlists",
            "href": "/v1/me/library/playlists/p.eoGxpgbtxAPJG6",
            "attributes": {
                "description": {
                    "standard": ""
                },
                "dateAdded": "2021-09-02T18: 43: 15Z",
                "hasCatalog": true,
                "isPublic": true,
                "playParams": {
                    "id": "p.eoGxpgbtxAPJG6",
                    "kind": "playlist",
                    "isLibrary": true,
                    "globalId": "pl.u-WabZ6rRCYW2vBE"
                },
                "name": "Chill Tracks Instrumental",
                "canEdit": true
            }
        },
        {
            "id": "p.4Y0JJrJuMWkD60",
            "type": "library-playlists",
            "href": "/v1/me/library/playlists/p.4Y0JJrJuMWkD60",
            "attributes": {
                "description": {
                    "standard": ""
                },
                "dateAdded": "2022-03-10T02: 26: 39Z",
                "hasCatalog": true,
                "isPublic": false,
                "playParams": {
                    "id": "p.4Y0JJrJuMWkD60",
                    "kind": "playlist",
                    "isLibrary": true,
                    "globalId": "pl.u-kv9llBlC6XZWBv"
                },
                "name": "Chill Tracks w/ Vocals",
                "canEdit": true
            }
        }
    ],
    "meta": {
        "total": 3
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

Get Multiple Library Playlist Folders

Fetch one or more library playlist folders by using their identifiers.

Create a New Library Playlist Folder

Create a new playlist folder in a user’s library.

object LibraryPlaylistFolderCreationRequest

Request object to create a new library playlist folder.

