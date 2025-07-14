

- Apple Music API
-  Get Multiple Library Artists 

Web Service Endpoint

# Get Multiple Library Artists

Fetch one or more library artists by using their identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/me/library/artists
```

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the artists. The maximum fetch limit is 25.

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

LibraryArtistsResponse

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
https://api.music.apple.com/v1/me/library/artists?ids=r.y8mMT7t
```

```
{
    "data": [
        {
            "id": "r.y8mMT7t",
            "type": "library-artists",
            "href": "/v1/me/library/artists/r.y8mMT7t",
            "attributes": {
                "name": "Orville Peck"
            }
        }
    ]
}
```

## See Also

### Related Documentation

object LibraryArtists

A resource object that represents an artist present in a user’s library.

object LibraryArtistsResponse

The response to a library artists request.

### Requesting a Library Artist

Get a Library Artist

Fetch a library artist by using its identifier.

Get a Library Artist's Relationship Directly by Name

Fetch a library artist’s relationship by using its identifier.

Get All Library Artists

Fetch all the library artists in alphabetical order.

