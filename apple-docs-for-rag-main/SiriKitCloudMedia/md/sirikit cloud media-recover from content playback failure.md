

- SiriKit Cloud Media
-  Recover from Content Playback Failure 

Web Service Endpoint

# Recover from Content Playback Failure

Provide a recovery queue that allows the client to resume playback after an error.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/queues/contentPlaybackFailure
```

## Header Parameters

`Accept-Language`

`string`

The client’s current user interface language. If possible, respond with localized content for this language.

`User-Agent`

`string`

 (Required) 

The client’s extension protocol. This is an RFC 7231-compliant string that contains the product name `AppleCloudExtension` and the version of the SiriKit extension library that’s running on the client.

Maximum length: `250`

Value: `/AppleCloudExtension/([0-9]+\.[0-9]+\.[0-9]+) *.*/`

`x-applecloudextension-retry-count`

`uint32`

The number of previous requests from the client. The client omits this header on the first attempt.

Minimum: `1`

`x-applecloudextension-session-id`

`string`

 (Required) 

A session identifier to pair each request and response. Respond to requests with the value the client provides.

Minimum length: `1`

Maximum length: `128`

## HTTP Body

ContentPlaybackFailureRequest

A JSON object that describes the playback failure, the state of the current queue, and the constraints to apply to the recovery queue.

Content-Type: application/json

## Response Codes

` 200 ``OK`

Queue

`OK`

The request is successful.

Content-Type: application/json

` 204 ``No Content`

`No Content`

The service is unable to provide a recovery queue segment.

` 401 ``Unauthorized`

`Unauthorized`

The request requires authorization. The client can attempt to reauthorize and then retry the request.

` 410 ``Gone`

`Gone`

The request includes an expired UserActivity, which the service is unable to use to provide a recovery queue segment.

## Discussion

If the playback of a queue fails to start, or there’s an error during playback that the client can recover from, the client reports the failure by sending a request to this endpoint. Configure your service to respond with a recovery queue that the client can use to restart playback.

Examples of recoverable playback failures include:

- The client is unable to load the media using the provided URL.

- The client is unable to acquire a content key for a protected asset.

- The number of items in the queue segment exceeds the configured maximum.

## See Also

### Playback Failure

object ContentFailure

An object that describes why the client can’t play a specific piece of content.

object ContentPlaybackFailureRequest

A request the client sends to recover from failed content playback.

object ContentPlaybackFailureResponse

A response that allows the client to recover from failed content playback.

