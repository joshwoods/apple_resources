

- SiriKit Cloud Media
- PlayMediaMediaItemResolutionResult
-  PlayMediaMediaItemResolutionResult.ConfirmationRequired 

Object

# PlayMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaMediaItemResolutionResult.ConfirmationRequired
```

## Properties

`mediaItemToConfirm`

MediaItem

 (Required) 

A media item for the user to confirm or reject.

## Discussion

Prefer to provide a successful result, even if you aren’t sure that you’re identifying the media item accurately. The user can cancel playback and try asking again.

## See Also

### Specifying a Result

object PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object PlayMediaMediaItemResolutionResult.Unsupported

The reason your service can’t play the requested media item.

object PlayMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

