

- SiriKit Cloud Media
-  Process an Update Media Affinity Intent 

Web Service Endpoint

# Process an Update Media Affinity Intent

Record the user’s preference for a specific media item or a broader category of media.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/intent/updateMediaAffinity
```

## Header Parameters

`Accept-Language`

`string`

 (Required) 

The client’s current user interface language. Respond with localized content for this language, if available.

`Request-Timeout`

`uint32`

 (Required) 

An approximate deadline, in seconds, for processing this real-time user request. The Session object provides the exact deadline for handling an intent.

Minimum: `1`

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

`[`UpdateMediaAffinityIntentHandlingInvocation`]`

An array of requests to process intents.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`[`UpdateMediaAffinityIntentHandlingInvocationResponse`]`

`OK`

The request succeeds.

Content-Type: application/json

## Topics

### Processing an Update Media Affinity Intent

object UpdateMediaAffinityIntent

An object that describes a user’s stated preference regarding media items.

object UpdateMediaAffinityIntentHandlingInvocation

A request to process an update media affinity intent.

type UpdateMediaAffinityIntentHandlingInvocationResponse

The service’s response to a request to process an update media affinity intent.

### Identifying the Intended Media Items

object UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

object UpdateMediaAffinityMediaItemResolutionResult

A media item that matches an update media affinity intent, or information about why your service can’t provide a media item.

type UpdateMediaAffinityMediaItemUnsupportedReason

Reasons the media service can’t update information about the media item.

### Discerning Like or Dislike

type MediaAffinityType

A preference or dislike for a media item.

object UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse

Your service’s response to a request that expresses a preference or dislike for a media item.

object MediaAffinityTypeResolutionResult

A media affinity that matches an update media affinity intent, or information about why your service can’t determine the media affinity.

### Handling an Update Media Affinity Intent

object UpdateMediaAffinityIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved update media affinity intent.

object UpdateMediaAffinityIntentResponse

A structure that contains a response code indicating how your service handles an update media affinity intent.

type UpdateMediaAffinityIntentResponseCode

Codes your service can return when handling an update media affinity intent.

## See Also

### Playback Events

type QueueActivityReportEvent

An event that occurs during content playback.

Report Playback Progress and Activity

Monitor progress through the playback queue.

object UpdateActivityRequest

A report of the client’s current playback state and recent user interaction, and an opportunity for your service to modify the client’s playback queue.

object UpdateActivityResponse

Updates to the client’s queue and user activity in response to a report of playback progress.

