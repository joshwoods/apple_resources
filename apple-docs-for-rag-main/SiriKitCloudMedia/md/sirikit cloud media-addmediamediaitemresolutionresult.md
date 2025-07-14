

- SiriKit Cloud Media
-  AddMediaMediaItemResolutionResult 

Object

# AddMediaMediaItemResolutionResult

A media item that matches an add media intent, or information about why your service can’t provide a media item.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaMediaItemResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `AddMediaMediaItemResolutionResult`

`success`

AddMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

`confirmationRequired`

AddMediaMediaItemResolutionResult.ConfirmationRequired

A media item for the user to confirm.

`disambiguation`

AddMediaMediaItemResolutionResult.Disambiguation

Multiple media items for the user to choose from.

`unsupported`

AddMediaMediaItemResolutionResult.Unsupported

Information about why your service can’t resolve the media item.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Providing a Media Item

object AddMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

### Reporting a Problem

object AddMediaMediaItemResolutionResult.Unsupported

The reason your service can’t add the media item to the user’s library or to a playlist.

type AddMediaMediaItemUnsupportedReason

Reasons the media service can’t add the media item to the user’s library or to a playlist.

### Clarifying a Possible Match

object AddMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before you add it to their library or to a playlist.

object AddMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose which media item they want to add to their library or to a playlist.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Identifying a Media Item

object AddMediaIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

