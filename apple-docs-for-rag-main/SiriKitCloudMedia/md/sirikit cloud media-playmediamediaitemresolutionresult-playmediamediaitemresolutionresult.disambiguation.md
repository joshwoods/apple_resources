

- SiriKit Cloud Media
- PlayMediaMediaItemResolutionResult
-  PlayMediaMediaItemResolutionResult.Disambiguation 

Object

# PlayMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaMediaItemResolutionResult.Disambiguation
```

## Properties

`mediaItemsToDisambiguate`

`[`MediaItem`]`

 (Required) 

Media items that might match the user’s intent.

## See Also

### Specifying a Result

object PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object PlayMediaMediaItemResolutionResult.Unsupported

The reason your service can’t play the requested media item.

object PlayMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

