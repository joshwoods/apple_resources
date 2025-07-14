

- Device Management
-  Get Multiple Genres 

Web Service Endpoint

# Get Multiple Genres

Fetch metadata for genres from the catalog by using their identifiers.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://api.ent.apple.com/v1/catalog/{storefront}/genres#ids
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefrontobjects`.

## Query Parameters

`ids`

`[string]`

 (Required) 

The unique identifiers for the genres.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## Response Codes

` 200 ``OK`

GenresResponse

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

A response indicating an incorrect `Authorization` header.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

A response indicating an error occurred on the server.

Content-Type: application/json

## Discussion

### Example

- Request
- Response

```
```

```
```

## Topics

### Responses

object GenresResponse

object UnauthorizedResponse

A response that indicates an incorrect authorization header.

object ErrorsResponse

The collection of errors that occurred while processing the request.

## See Also

### Endpoints

Fetch a apps resource's relationship

Fetch a books resource's relationship

Get a Genre

Fetch metadata for a genre from the catalog by using its identifier.

