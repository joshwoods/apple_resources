

- SiriKit Cloud Media
- UpdateMediaAffinityMediaItemResolutionResult
-  UpdateMediaAffinityMediaItemResolutionResult.Disambiguation 

Object

# UpdateMediaAffinityMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityMediaItemResolutionResult.Disambiguation
```

## Properties

`mediaItemsToDisambiguate`

`[`MediaItem`]`

 (Required) 

Media items that might match the user’s intent.

## See Also

### Specifying the Result

object UpdateMediaAffinityMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object UpdateMediaAffinityMediaItemResolutionResult.Unsupported

The reason your service can’t update information about the requested media item.

object UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

