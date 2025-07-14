

- Apple Music API
-  Get Equivalent Catalog Music Videos by ID 

Web Service Endpoint

# Get Equivalent Catalog Music Videos by ID

Fetch the equivalent, available content in the storefront for the provided music videos’ identifiers.

Apple Music 1.0+

## URL

``` source
GET https://api.music.apple.com/v1/catalog/{storefront}/music-videos
```

## Path Parameters

`storefront`

`string`

 (Required) 

An iTunes Store territory, specified by an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefront` objects.

## Query Parameters

`filter[equivalents]`

`[string]`

 (Required) 

A filter to apply to the request. The maximum fetch limit is 25.

`include`

`[string]`

Additional relationships to include in the fetch.

`l`

`string`

The localization to use, specified by a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object specified by `storefront`. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`restrict`

`[string]`

A set of restrictions (for example, to restrict explicit content).

Value: `explicit`

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

## Response Codes

` 200 ``OK`

MusicVideosResponse

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
https://api.music.apple.com/v1/catalog/ch/music-videos?filter[equivalents]=1553279848
```

```
{
    "data": [
        {
            "id": "1552406856",
            "type": "music-videos",
            "href": "/v1/catalog/ch/music-videos/1552406856",
            "attributes": {
                "previews": [
                    {
                        "url": "https: //video-ssl.itunes.apple.com/itunes-assets/Video114/v4/d6/33/c5/d633c5de-0ddb-ad5d-a560-3e9fb35c057b/mzvf_2101846033664580247.720w.h264lc.U.p.m4v",
                        "hlsUrl": "https: //play.itunes.apple.com/WebObjects/MZPlay.woa/hls/playlist.m3u8?cc=CH&a=1552406856&id=230060134&l=de&aec=HD",
                        "artwork": {
                            "width": 1561,
                            "url": "https: //is2-ssl.mzstatic.com/image/thumb/Video114/v4/f0/dc/be/f0dcbea2-4718-c310-d9f6-f16d86ffd699/Jobfaa18d62-b9d3-4e7a-ac99-fc4ca04a9c9a-109210777-PreviewImage_preview_image_45000_video_sdr-Time1612539991665.png/{w}x{h}bb.jpeg",
                            "height": 1080,
                            "textColor3": "a5a69c",
                            "textColor2": "bac0c4",
                            "textColor4": "9a9fa1",
                            "textColor1": "c7c9bd",
                            "bgColor": "1b1b19",
                            "hasP3": false
                        }
                    }
                ],
                "artwork": {
                    "width": 1553,
                    "url": "https: //is1-ssl.mzstatic.com/image/thumb/Video114/v4/c4/09/a5/c409a5d5-61c1-5a3b-54ca-6bb34af4a7da/21UMGIM09694.crop.jpg/{w}x{h}mv.jpeg",
                    "height": 1072,
                    "textColor3": "c6b490",
                    "textColor2": "d4bb93",
                    "textColor4": "b9a17e",
                    "textColor1": "e5d2a9",
                    "bgColor": "4d3a2c",
                    "hasP3": false
                },
                "artistName": "Dua Lipa",
                "url": "https: //music.apple.com/ch/music-video/were-good/1552406856",
                "genreNames": [
                    "Pop"
                ],
                "has4K": false,
                "durationInMillis": 181033,
                "releaseDate": "2021-02-12",
                "name": "We’re Good",
                "isrc": "GB1302001140",
                "playParams": {
                    "id": "1552406856",
                    "kind": "musicVideo"
                },
                "hasHDR": false
            },
            "relationships": {
                "artists": {
                    "href": "/v1/catalog/ch/music-videos/1552406856/artists",
                    "data": [
                        {
                            "id": "1031397873",
                            "type": "artists",
                            "href": "/v1/catalog/ch/artists/1031397873"
                        }
                    ]
                },
                "albums": {
                    "href": "/v1/catalog/ch/music-videos/1552406856/albums",
                    "data": []
                }
            }
        }
    ],
    "meta": {
        "filters": {
            "equivalents": {
                "1553279848": [
                    {
                        "id": "1552406856",
                        "type": "music-videos",
                        "href": "/v1/catalog/ch/music-videos/1552406856"
                    }
                ]
            }
        }
    }
}

```

## See Also

### Related Documentation

object MusicVideos

A resource object that represents a music video.

object MusicVideosResponse

The response to a music videos request.

### Requesting a Catalog Music Video

Get a Catalog Music Video

Fetch a music video by using its identifier.

Get a Catalog Music Video's Relationship Directly by Name

Fetch a music video’s relationship by using its identifier.

Get a Catalog Music Video’s Relationship View Directly by Name

Fetch related resources for a single music video’s relationship view.

Get Multiple Catalog Music Videos by ID

Fetch one or more music videos by using their identifiers.

Get Multiple Catalog Music Videos by ISRC

Fetch one or more music videos by using their International Standard Recording Code (ISRC) values.

