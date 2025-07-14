

- SiriKit Cloud Media
-  Report Playback Progress and Activity 

Web Service Endpoint

# Report Playback Progress and Activity

Monitor progress through the playback queue.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/queues/updateActivity
```

## Header Parameters

`Accept-Language`

`string`

 (Required) 

The client’s current user interface language. Respond with localized content for this language, if available.

`User-Agent`

`string`

 (Required) 

The extension protocol running on the client. This is an RFC 7231-compliant string that contains the product name *AppleCloudExtension* and the SiriKit Extension library version running on the client.

Maximum length: `250`

Value: `/AppleCloudExtension/([0-9]+\.[0-9]+\.[0-9]+) *.*/`

`x-applecloudextension-retry-count`

`uint32`

The number of previous requests from the client. The client omits this header on the first attempt.

Minimum: `1`

`x-applecloudextension-session-id`

`string`

 (Required) 

A constant session identifier to include in each request and response. Respond to each request with the session ID the client sends in that request.

Minimum length: `1`

Maximum length: `128`

## HTTP Body

UpdateActivityRequest

The most recent state of the client’s playback queue.

Content-Type: application/json

## Response Codes

` 200 ``OK`

UpdateActivityResponse

`OK`

The request succeeds, and the response includes an updated UserActivity or Queue.

Content-Type: application/json

` 204 ``No Content`

`No Content`

The request succeeds, and the client can continue to use its current UserActivity and playback queue.

` 401 ``Unauthorized`

`Unauthorized`

The request requires authorization. The client may attempt to reauthorize and then retry.

` 404 ``Not Found`

`Not Found`

The provided QueueIdentifier doesn’t match any current queue, or is permanently expired. The client may still use its current UserActivity to request a new queue.

` 410 ``Gone`

`Gone`

The request’s UserActivity is permanently expired and invalid for requesting a queue.

## See Also

### Playback Events

type QueueActivityReportEvent

An event that occurs during content playback.

object UpdateActivityRequest

A report of the client’s current playback state and recent user interaction, and an opportunity for your service to modify the client’s playback queue.

object UpdateActivityResponse

Updates to the client’s queue and user activity in response to a report of playback progress.

Process an Update Media Affinity Intent

Record the user’s preference for a specific media item or a broader category of media.

