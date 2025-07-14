

- SiriKit Cloud Media
-  ContentPlaybackFailureResponse 

Object

# ContentPlaybackFailureResponse

A response that allows the client to recover from failed content playback.

SiriKit Cloud Media 1.0.2+

``` source
object ContentPlaybackFailureResponse
```

## Properties

`version`

`string`

The version of the client’s `SiriKitMediaAPI` library.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

`queue`

Queue

The Queue segment the client uses to recover from the playback failure.

## See Also

### Playback Failure

Recover from Content Playback Failure

Provide a recovery queue that allows the client to resume playback after an error.

object ContentFailure

An object that describes why the client can’t play a specific piece of content.

object ContentPlaybackFailureRequest

A request the client sends to recover from failed content playback.

