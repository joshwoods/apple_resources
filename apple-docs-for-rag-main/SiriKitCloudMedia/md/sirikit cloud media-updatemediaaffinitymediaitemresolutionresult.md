

- SiriKit Cloud Media
-  UpdateMediaAffinityMediaItemResolutionResult 

Object

# UpdateMediaAffinityMediaItemResolutionResult

A media item that matches an update media affinity intent, or information about why your service can’t provide a media item.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityMediaItemResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `UpdateMediaAffinityMediaItemResolutionResult`

`success`

UpdateMediaAffinityMediaItemResolutionResult.Success

A media item that successfully matches the intent.

`confirmationRequired`

UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired

A media item for the user to confirm as a match.

`disambiguation`

UpdateMediaAffinityMediaItemResolutionResult.Disambiguation

Multiple media items for the user to choose from.

`unsupported`

UpdateMediaAffinityMediaItemResolutionResult.Unsupported

Information about why your service can’t resolve the media item.

## Topics

### Specifying the Result

object UpdateMediaAffinityMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object UpdateMediaAffinityMediaItemResolutionResult.Unsupported

The reason your service can’t update information about the requested media item.

object UpdateMediaAffinityMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

object UpdateMediaAffinityMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Identifying the Intended Media Items

object UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

type UpdateMediaAffinityMediaItemUnsupportedReason

Reasons the media service can’t update information about the media item.

