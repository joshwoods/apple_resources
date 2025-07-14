

- Apple News API
-  Read Channel Information 

Web Service Endpoint

# Read Channel Information

Get details about your channel, including the name, corresponding website, and default section.

Apple News API 1.0+

## URL

``` source
GET https://news-api.apple.com/channels/{channelId}
```

## Path Parameters

`channelId`

`string`

 (Required) 

The UUID of the channel to get. You can get your channel ID from News Publisher. See Use your CMS with News Publisher in News Publisher User Guide.

## Response Codes

` 200 ``OK`

ChannelResponse

`OK`

The request was successful.

Content-Type: application/json

` 400 ``Bad Request`

Error

`Bad Request`

- `MISSING`. You didn’t include the Channel UUID field in the request. Key path: \*

- `INVALID_JSON`. The server can’t parse the JSON specified in the request as JSON. Key path: None.

- `INVALID_TYPE`. The value you specified for `channelId` is not of the correct type for that field. Key path: `channelId`.

Content-Type: application/json

` 401 ``Unauthorized`

Error

`Unauthorized`

You didn’t include the `Authorization` header. Key path: None.

Content-Type: application/json

` 403 ``Forbidden`

Error

`Forbidden`

You tried to access a channel your `API` `key` doesn’t have permission to access. Key path: None.

Content-Type: application/json

` 404 ``Not Found`

Error

`Not Found`

- The endpoint you tried to access doesn’t exist. Key path: None.

- The channel you tried to access doesn’t exist. Key path: `channel_id.`

Content-Type: application/json

## Mentioned in 

Making an HTTP Request to the Apple News API

Signing the HTTP Request

## Discussion

Use the Read Channel Information endpoint to retrieve information about the channel, list of custom fonts used in the channel (Channel), and link to the channel’s default section (ChannelLinks). See Making an HTTP Request to the Apple News API and Signing the HTTP Request in Apple News API Tutorial.

You create a channel in News Publisher, not the Apple News API. See Add or share a channel in News Publisher User Guide.

### Example

- Request
- Response

```
GET /channels/63a75491-2c4d-3530-af91-819be8c3ace0 HTTP/1.1
Host: news-api.apple.com
Accept: application/json
Authorization: HHMAC; key="1e3gfc5e-e9f8-4232-a6be-17bf40edad09"; signature="mLtpym3Lgl1300t8cze9wyWOaxkRBKL3j3ztalMjgWs="; date="2015-03-05T02:49:58Z"
```

```
HTTP/1.1 200 OK
Date: Thu, 05 Mar 2015 02:53:54 GMT
Content-Type: application/json;charset=UTF-8
Transfer-Encoding: chunked  
{
  "data": {
    "createdAt": "2015-02-19T04:57:23Z",
    "modifiedAt": "2015-02-23T23:25:53Z",
    "id": "63a75491-2c4d-3530-af91-819be8c3ace0",
    "type": "channel",
    "shareUrl": "https://apple.news/ArRPpLPE9QXu3sehS0rvxvA",
    "links": {
      "defaultSection": "https://news-api.apple.com/sections/4523e2f6-89fb-4842-b9f2-46514f7ebc6b",
      "self": "https://news-api.apple.com/channels/63a75491-2c4d-3530-af91-819be8c3ace0"
    },
    "name": "My Channel",
    "website": "http://example.com"
    "fonts": [
    ]
  }
}
```

## See Also

### Channel

Read Channel Quota Information

Get details about your channel’s remaining quota for sending create and update requests, the queue size, and wait time.

object Channel

See the fields the read channel endpoint returned.

object ChannelLinks

See the links the read channel endpoint returned.

object ChannelResponse

See which objects make up the channel response.

