

- SiriKit Cloud Media
-  ContentPlaybackFailureRequest 

Object

# ContentPlaybackFailureRequest

A request the client sends to recover from failed content playback.

SiriKit Cloud Media 1.0.2+

``` source
object ContentPlaybackFailureRequest
```

## Properties

`constraints`

Constraints

 (Required) 

Limitations on the type and quantity of content to provide in the recovery Queue.

`contentFailure`

ContentFailure

 (Required) 

An object that describes why playback failed.

`nextContentUrl`

`string`

The URL the client uses to request the next queue segment.

Minimum length: `0`

Maximum length: `2000`

`previousContentUrl`

`string`

The URL the client uses to request the previous queue segment.

Minimum length: `0`

Maximum length: `2000`

`sessionIdentifier`

`string`

 (Required) 

The identifier that associates the requests and responses of a specific intent.

Minimum length: `1`

Maximum length: `128`

`timestamp`

`date-time`

The time when the playback failure occurred.

`userActivity`

UserActivity

A description of the client’s current playback queue.

`version`

`string`

 (Required) 

The version of the client’s `SiriKitMediaAPI` library.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

`whilePlaying`

PlayerContext

 (Required) 

The content that failed to play.

## Discussion

If the playback of a queue fails to start, or there’s an error during playback from which the client can recover, the client sends this request to your service to report the failure and retrieve a new queue.

## See Also

### Playback Failure

Recover from Content Playback Failure

Provide a recovery queue that allows the client to resume playback after an error.

object ContentFailure

An object that describes why the client can’t play a specific piece of content.

object ContentPlaybackFailureResponse

A response that allows the client to recover from failed content playback.

