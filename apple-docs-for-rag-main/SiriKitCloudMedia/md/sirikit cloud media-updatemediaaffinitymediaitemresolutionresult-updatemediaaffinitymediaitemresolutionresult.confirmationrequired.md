

- SiriKit Cloud Media
- UpdateMediaAffinityMediaItemResolutionResult
-  UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired 

Object

# UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired
```

## Properties

`mediaItemToConfirm`

MediaItem

 (Required) 

A media item for the user to confirm or reject.

## See Also

### Specifying the Result

object UpdateMediaAffinityMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object UpdateMediaAffinityMediaItemResolutionResult.Unsupported

The reason your service can’t update information about the requested media item.

object UpdateMediaAffinityMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

