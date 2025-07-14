

- Apple Music API
-  Get a Catalog Record Label 

Web Service Endpoint

# Get a Catalog Record Label

Fetch a record label by using its identifier.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/record-labels/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the record label.

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

`include`

`[string]`

Additional relationships to include in the fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`views`

`[string]`

The views to activate for the record label resource.

Possible Values: `latest-releases, top-releases`

## Response Codes

` 200 ``OK`

RecordLabelsResponse

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

If successful, the HTTP status code is 200 (OK) and the `data` array contains the requested resource object. If unsuccessful, the HTTP status code indicates the error and the details are in the `errors` array. For more information, see Handling Requests and Responses.

### Example

- Request
- Response

```
https://api.music.apple.com/v1/catalog/us/record-labels/1543990853
```

```
{
    "data": [
        {
            "id": "1543990853",
            "type": "record-labels",
            "href": "/v1/catalog/us/record-labels/1543990853",
            "attributes": {
                "artwork": {
                    "width": 1080,
                    "height": 1080,
                    "url": "https: //is3-ssl.mzstatic.com/image/thumb/Features114/v4/2b/20/be/2b20be3f-6f19-3701-074e-b233964caaa7/QkwtTVMtV1ctTmluamFfVHVuZS1BREFNX0lEPTE1NDM5OTA4NTMucG5n.png/{w}x{h}bb.jpg",
                    "bgColor": "111111",
                    "textColor1": "93c7d9",
                    "textColor2": "89b6c6",
                    "textColor3": "759caa",
                    "textColor4": "6d8f9b"
                },
                "description": {
                    "standard": "Ninja Tune—formed in 1990 by Matt Black and Jon More (Coldcut)—has established itself as one of the world’s leading independent record labels. Now it’s a bona fide global music institution, synonymous with diverse, uncompromising releases and equally visionary artists—from breaking to GRAMMY-nominated acts—committed to pushing the boundaries of music. (From the label)"
                },
                "name": "Ninja Tune",
                "url": "https: //music.apple.com/us/label/ninja-tune/1543990853"
            }
        }
    ]
}

```

## See Also

### Related Documentation

object RecordLabels

A resource object that represents a record label.

object RecordLabelsResponse

The response to a request for record labels.

### Requesting Catalog Record Labels

Get a Catalog Record Label’s Relationship View Directly by Name

Fetch related resources for a single record label’s relationship view.

Get Multiple Record Labels

Fetch one or more record labels by using their identifiers.

