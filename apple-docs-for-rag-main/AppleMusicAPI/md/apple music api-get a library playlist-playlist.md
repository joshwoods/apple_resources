

- Apple Music API
-  Get a Library Playlist 

Web Service Endpoint

# Get a Library Playlist

Fetch a library playlist by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/playlists/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the library playlist.

## Query Parameters

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`include`

`[string]`

Additional relationships to include in the fetch.

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

LibraryPlaylistsResponse

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
https://api.music.apple.com/v1/me/library/playlists/p.ldvAAZ3C3Qmop9
```

```
{
    "data": [
        {
            "id": "p.ldvAAZ3C3Qmop9",
            "type": "library-playlists",
            "href": "/v1/me/library/playlists/p.ldvAAZ3C3Qmop9",
            "attributes": {
                "playParams": {
                    "id": "p.ldvAAZ3C3Qmop9",
                    "kind": "playlist",
                    "isLibrary": true,
                    "globalId": "pl.cb4d1c09a2df4230a78d0395fe1f8fde"
                },
                "canEdit": false,
                "name": "Piano Chill",
                "description": {
                    "standard": "Discover the liberating power of the piano with pieces chosen by Dirk Maassen."
                },
                "dateAdded": "2021-09-30T00: 55: 48Z",
                "artwork": {
                    "width": null,
                    "height": null,
                    "url": "https: //is3-ssl.mzstatic.com/image/thumb/Features125/v4/dc/47/7c/dc477c6f-9029-bd1c-8e89-87b04042a55b/U0MtTVMtV1ctUGlhbm9fQ2hpbGwtQURBTV9JRD0xMDcyODMxMzA0LnBuZw.png/{w}x{h}SC.DN01.jpeg"
                },
                "isPublic": false,
                "hasCatalog": true
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

### Requesting a Library Playlist

Get a Library Playlist's Relationship Directly by Name

Fetch a library playlist’s relationship by using its identifier.

Get Multiple Library Playlists

Fetch one or more library playlists by using their identifiers.

Get All Library Playlists

Fetch all the library playlists in alphabetical order.

