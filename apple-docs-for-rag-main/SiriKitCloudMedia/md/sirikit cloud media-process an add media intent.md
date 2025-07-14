

- SiriKit Cloud Media
-  Process an Add Media Intent 

Web Service Endpoint

# Process an Add Media Intent

Add media items to the user’s library or to a playlist.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/intent/addMedia
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

The number of previous requests from the client.

Minimum: `1`

`x-applecloudextension-session-id`

`string`

 (Required) 

A constant session identifier to include in each request and response. Respond to each request with the same session ID the client sends in that request.

Minimum length: `1`

Maximum length: `128`

## HTTP Body

`[`AddMediaIntentHandlingInvocation`]`

An array of requests to process intents.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`[`AddMediaIntentHandlingInvocationResponse`]`

`OK`

The request is successful.

Content-Type: application/json

## Discussion

Processing a request to add media items to the user’s library or to a playlist requires a few steps: resolving the intended media item, resolving the intended destination library or playlist, confirming the intent, and handling the intent.

You can often improve the overall response time to the user’s request by providing multiple responses to the client’s first request. Include an AddMediaIntentHandlingInvocationResponse for each of the subsequent steps in your response to the first request of a session. This allows the client to skip subsequent requests when you can resolve each parameter successfully. If your service responds with a disambiguation, confirmation, or failure, the client disregards the pre-emptive responses, and sends the subsequent intent-processing requests.

## Topics

### Processing an Add Media Intent

object AddMediaIntent

An object that describes the user’s request to add media items to their library or to a specific playlist.

object AddMediaIntentHandlingInvocation

A request to process an add media intent.

type AddMediaIntentHandlingInvocationResponse

The service’s response to a request to process an add media intent.

### Identifying a Media Item

object AddMediaIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

object AddMediaMediaItemResolutionResult

A media item that matches an add media intent, or information about why your service can’t provide a media item.

### Identifying a Library or Playlist

object AddMediaIntentHandlingResolveMediaDestinationInvocationResponse

Your service’s response to a request to resolve media items in an add media intent.

object AddMediaMediaDestinationResolutionResult

The user’s library or a specified playlist, or information about why your service can’t use the requested destination.

### Confirming and Handling an Add Media Intent

object AddMediaIntentResponse

A structure that contains a response code indicating your service’s progress in handling an add media intent.

type AddMediaIntentResponseCode

Codes your service can return when confirming or handling an add media intent.

object AddMediaIntentHandlingConfirmInvocationResponse

The service’s response to a request to confirm an add media intent.

object AddMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved add media intent.

