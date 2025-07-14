

- SiriKit Cloud Media
- PlayMediaMediaItemResolutionResult
-  PlayMediaMediaItemResolutionResult.Unsupported 

Object

# PlayMediaMediaItemResolutionResult.Unsupported

The reason your service can’t play the requested media item.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaMediaItemResolutionResult.Unsupported
```

## Properties

`reason`

PlayMediaMediaItemUnsupportedReason

The reason your service can’t play the requested media item.

## Discussion

If you can’t find the media item the user specifies, don’t provide a reason. When the client receives an `Unsupported` object without a reason, it provides a generic failure message to the user.

## See Also

### Specifying a Result

object PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object PlayMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

object PlayMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

