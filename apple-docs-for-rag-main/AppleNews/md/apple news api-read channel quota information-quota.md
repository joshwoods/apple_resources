

- Apple News API
-  Read Channel Quota Information 

Web Service Endpoint

# Read Channel Quota Information

Get details about your channel’s remaining quota for sending create and update requests, the queue size, and wait time.

Apple News API 2.1+

## URL

``` source
GET https://news-api.apple.com/channels/{channelId}/quota
```

## Path Parameters

`channelId`

`string`

 (Required) 

The UUID of the channel. You can get your channel ID from News Publisher. See Use your CMS with News Publisher in News Publisher User Guide.

## Response Codes

` 200 ``OK`

Throttling

`OK`

The request was successful.

Content-Type: application/json

` 400 ``Bad Request`

Error

`Bad Request`

`MISSING`. You didn’t include the Channel UUID field in the request. Key path: \*

Content-Type: application/json

` 401 ``Unauthorized`

Error

`Unauthorized`

You didn’t include the `Authorization` header. Key path: None.

Content-Type: application/json

` 403 ``Forbidden`

Error

`Forbidden`

You tried to access a channel your API key doesn’t have permission to access. Key path: None.

Content-Type: application/json

` 404 ``Not Found`

Error

`Not Found`

- The endpoint you tried to access doesn’t exist. Key path: None.

- The channel you tried to access doesn’t exist. Key path: `channel_id`.

Content-Type: application/json

## Discussion

A Read Channel Quota Information request returns the publisher’s remaining create and update request quota, the queue size, and estimated wait time. This information is also available through the Meta object when you use the Create an Article and Update an Article endpoints.

### Example

- Request
- Response

```
GET /channels/63a75491-2c4d-3530-af91-819be8c3ace0/quota
Host: news-api.apple.com
Accept: application/json
Authorization: HHMAC; key="1e3gfc5e-e9f8-4232-a6be-17bf40edad09"; signature="mLtpym3Lgl1300t8cze9wyWOaxkRBKL3j3ztalMjgWs="; date="2015-03-05T02:49:58Z"
```

```
HTTP/1.1 200 OK
Date: Tue, 28 May 2019 20:40:29 GMT
Request-Id: d4ef2ad0-8188-11e9-ac39-815bb6436c0b
Content-Type: application/json;charset=utf-8
Transfer-Encoding: chunked
{
    "isThrottled": false,
    "queueSize": 0,
    "estimatedDelayInSeconds": 0,
    "quotaAvailable": 200
}
```

## See Also

### Channel

Read Channel Information

Get details about your channel, including the name, corresponding website, and default section.

object Channel

See the fields the read channel endpoint returned.

object ChannelLinks

See the links the read channel endpoint returned.

object ChannelResponse

See which objects make up the channel response.

