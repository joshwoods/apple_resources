

- Apple Music API
-  Get the User's Personal Apple Music Station 

Web Service Endpoint

# Get the User's Personal Apple Music Station

Fetch the current user’s personal Apple Music station.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/stations#filter-personal-station
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`filter[identity]`

`[string]`

 (Required) 

A filter to apply to the request.

Value: `personal`

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

StationsResponse

`OK`

A list of attribute extensions to apply to resources in the response.

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains the requested resource object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/stations?filter[identity]=personal
```

```
{
    "data": [
        {
            "id": "ra.u-741b035f6f0a85c81abb70ff757aa95f",
            "type": "stations",
            "href": "/v1/catalog/us/stations/ra.u-741b035f6f0a85c81abb70ff757aa95f",
            "attributes": {
                "artwork": {
                    "width": 2400,
                    "height": 2400,
                    "url": "https: //is1-ssl.mzstatic.com/image/thumb/Features124/v4/7b/1d/f0/7b1df048-0017-8ac0-98c9-735f14849606/mza_7507996640781423701.png/{w}x{h}bb.jpg"
                },
                "name": "My Station",
                "mediaKind": "audio",
                "playParams": {
                    "id": "ra.u-741b035f6f0a85c81abb70ff757aa95f",
                    "kind": "radioStation",
                    "format": "tracks",
                    "stationHash": "CgoIByIGCPeqnL8HEAE",
                    "hasDrm": false,
                    "mediaType": 0
                },
                "url": "https: //music.apple.com/us/station/grace-lis-station/ra.u-741b035f6f0a85c81abb70ff757aa95f",
                "isLive": false
            }
        }
    ],
    "meta": {
        "filters": {
            "identity": {
                "personal": [
                    {
                        "id": "ra.u-741b035f6f0a85c81abb70ff757aa95f",
                        "type": "stations",
                        "href": "/v1/catalog/us/stations/ra.u-741b035f6f0a85c81abb70ff757aa95f"
                    }
                ]
            }
        }
    }
}

```

## See Also

### Related Documentation

object Stations

A resource object that represents a station.

object StationsResponse

The response to a stations request.

### Requesting a Catalog Station

Get a Catalog Station

Fetch a station by using its identifier.

Get a Catalog Station's Relationship Directly by Name

Fetch a station’s relationship using its identifier.

Get Multiple Catalog Stations

Fetch one or more stations by using their identifiers.

Get the Apple Music Live Radio Stations

Fetch the Apple Music live radio stations for the storefront.

