

- SiriKit Cloud Media
- UpdateMediaAffinityMediaItemResolutionResult
-  UpdateMediaAffinityMediaItemResolutionResult.Success 

Object

# UpdateMediaAffinityMediaItemResolutionResult.Success

A media item that successfully matches the intent.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityMediaItemResolutionResult.Success
```

## Properties

`resolvedMediaItem`

MediaItem

 (Required) 

The song, album, podcast, or other media item that the user expresses a preference for.

## See Also

### Specifying the Result

object UpdateMediaAffinityMediaItemResolutionResult.Unsupported

The reason your service can’t update information about the requested media item.

object UpdateMediaAffinityMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

object UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

