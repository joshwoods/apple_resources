

- SiriKit Cloud Media
-  Get a Media Queue 

Web Service Endpoint

# Get a Media Queue

Provide a playback queue from a successfully processed play media intent.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/queues/playMedia
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

PlayMediaRequest

A UserActivity and constraints for the queue your service provides.

Content-Type: application/json

## Response Codes

` 200 ``OK`

Queue

`OK`

The request is successful.

Content-Type: application/json

` 204 ``No Content`

`No Content`

No more content exists for the requested queue.

` 401 ``Unauthorized`

`Unauthorized`

The request requires authorization. The client may attempt to reauthorize and then retry.

` 410 ``Gone`

`Gone`

The request’s UserActivity is permanently expired and invalid for requesting a queue.

## Discussion

There isn’t a default path for this endpoint. Specify the URL for this endpoint in your ExtensionConfig.Media.Queues.PlayMedia object.

## Topics

### Receiving a Queue Request

object PlayMediaRequest

A request for a media playback queue.

### Creating or Updating a Playback Queue

object Queue

A sequence of media content for playback, with links to the previous and next segments of a full playback queue.

type QueueIdentifier

A stable identifier for a playback queue.

object QueueInsertPointer

Instructions for editing the current playback queue.

object QueuePlayPointer

A position within a playback queue.

### Providing Queue Items

object Content

A description of a piece of playback content, such as a song, podcast, or advertisement.

type ContentIdentifier

An identifier for a song, podcast, ad, or other media content. The identifier must be stable and unique within a queue.

object ContentAttributes

Metadata for some media content.

### Customizing Playback Controls

object QueueControlMapping

A dictionary of configuration names and the media controls they permit.

object PlayMediaControl

A configuration for permitted user interactions and other player behaviors during playback.

type PlayMediaControlScheme

Default playback controls and settings for common content types.

object PlayMediaControlCommandSet

A set of modifications to apply to the default set of available playback controls.

## See Also

### Media Play Queues

Process a Play Media Intent

Interpret the user’s request to play a media item, and provide instructions to access a corresponding playback queue.

