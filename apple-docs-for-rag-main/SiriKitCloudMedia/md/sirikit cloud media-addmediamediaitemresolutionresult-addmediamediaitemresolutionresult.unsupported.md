

- SiriKit Cloud Media
- AddMediaMediaItemResolutionResult
-  AddMediaMediaItemResolutionResult.Unsupported 

Object

# AddMediaMediaItemResolutionResult.Unsupported

The reason your service can’t add the media item to the user’s library or to a playlist.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaMediaItemResolutionResult.Unsupported
```

## Properties

`reason`

AddMediaMediaItemUnsupportedReason

The reason your service can’t add the media item to the user’s library or to a playlist.

## Discussion

If you can’t find the media item the user specifies, don’t provide a reason. When the client receives an AddMediaMediaItemResolutionResult.Unsupported object without a reason, the client provides a generic failure message to the user.

## See Also

### Reporting a Problem

type AddMediaMediaItemUnsupportedReason

Reasons the media service can’t add the media item to the user’s library or to a playlist.

