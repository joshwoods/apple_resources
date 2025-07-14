

- Apple Music API
-  Add a Resource to a Library 

Web Service Endpoint

# Add a Resource to a Library

Add a catalog resource to a user’s iCloud Music Library.

Apple Music 1.0+

## URL

``` source
POST https://api.music.apple.com/v1/me/library
```

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique catalog identifiers for the resources. To indicate the type of resource to add, follow the `ids` with one of the allowed values. Add multiple types in the same request.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object that `storefront` specifies. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## Response Codes

` 202 ``Accepted`

EmptyBodyResponse

`Accepted`

Although the modification request was acceptable, it may not have completed.

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

If successful, the HTTP status code is 202 (Accepted) and there is no response body. For requested IDs that can’t be added to a user’s library, Apple Music Library ignores those IDs. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array.

This endpoint requires a music user token. For more information, see User Authentication for MusicKit.

Note

There may be a delay before a new resource appears in a user’s library.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/me/library?ids[albums]=1577502911
```

```
```

## See Also

### Related Documentation

object Resource

A resource—such as an album, song, or playlist.

