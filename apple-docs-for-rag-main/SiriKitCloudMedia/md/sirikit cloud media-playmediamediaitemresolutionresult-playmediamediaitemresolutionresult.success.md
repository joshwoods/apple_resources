

- SiriKit Cloud Media
- PlayMediaMediaItemResolutionResult
-  PlayMediaMediaItemResolutionResult.Success 

Object

# PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaMediaItemResolutionResult.Success
```

## Properties

`resolvedMediaItem`

MediaItem

 (Required) 

The song, album, podcast, or other media item that the user wants to play.

## See Also

### Specifying a Result

object PlayMediaMediaItemResolutionResult.Unsupported

The reason your service can’t play the requested media item.

object PlayMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

object PlayMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

