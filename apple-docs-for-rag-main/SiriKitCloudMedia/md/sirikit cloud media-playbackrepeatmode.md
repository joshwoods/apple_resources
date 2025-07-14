

- SiriKit Cloud Media
-  PlaybackRepeatMode 

Type

# PlaybackRepeatMode

The possible repeat modes for a media queue.

SiriKit Cloud Media 1.0.2+

``` source
string PlaybackRepeatMode
```

## Possible Values 

`none`  

Don’t repeat media items.

`all`  

Repeat all media items within the playback queue.

`one`  

Repeat the current media item.

`unknown`  

An unknown repeat mode.

## See Also

### Resolving the Intended Repeat Mode

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse

Your service’s response to a request to resolve the repeat mode in a play media intent.

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse.Result

The result of resolving the repeat mode for a play media intent.

object PlaybackRepeatModeResolutionResult

Information about whether your service can identify the specified repeat mode.

