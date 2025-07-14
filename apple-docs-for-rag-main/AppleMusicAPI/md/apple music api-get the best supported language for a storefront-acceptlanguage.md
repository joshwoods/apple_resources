

- Apple Music API
-  Get the best supported language for a storefront 

Web Service Endpoint

# Get the best supported language for a storefront

Fetch the best supported language for a storefront from a list.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/language/{storefront}/tag
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`acceptLanguage`

`[string]`

 (Required) 

A list of languages to accept.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

## Response Codes

` 200 ``OK`

LangageTagResponse

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
https://api.music.apple.com/v1/language/us/tag?acceptLanguage=en-US
```

```
{
    “results”: {
        “tag”: “en-US”
    }
}
```

