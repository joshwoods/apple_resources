

- SiriKit Cloud Media
-  PlayMediaMediaItemResolutionResult 

Object

# PlayMediaMediaItemResolutionResult

A media item that matches a play media intent, or information about why your service can’t provide a media item.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaMediaItemResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `PlayMediaMediaItemResolutionResult`

`success`

PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

`confirmationRequired`

PlayMediaMediaItemResolutionResult.ConfirmationRequired

A media item for the user to confirm as a match.

`disambiguation`

PlayMediaMediaItemResolutionResult.Disambiguation

Multiple media items for the user to choose from.

`unsupported`

PlayMediaMediaItemResolutionResult.Unsupported

Information about why your service can’t resolve the media item.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `unsupported` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Specifying a Result

object PlayMediaMediaItemResolutionResult.Success

A media item that successfully matches the intent.

object PlayMediaMediaItemResolutionResult.Unsupported

The reason your service can’t play the requested media item.

object PlayMediaMediaItemResolutionResult.Disambiguation

A result that requires the user to choose from multiple media items before proceeding.

object PlayMediaMediaItemResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media item before proceeding.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Resolving a Media Item

object PlayMediaIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in a play media intent.

type PlayMediaMediaItemUnsupportedReason

Reasons the media service can’t play the media item.

