

- SiriKit Cloud Media
-  AddMediaMediaDestinationResolutionResult 

Object

# AddMediaMediaDestinationResolutionResult

The user’s library or a specified playlist, or information about why your service can’t use the requested destination.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaMediaDestinationResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `AddMediaMediaDestinationResolutionResult`

`success`

AddMediaMediaDestinationResolutionResult.Success

The user’s library or a playlist that successfully matches the intent.

`unsupported`

AddMediaMediaDestinationResolutionResult.Unsupported

Information about why your service can’t resolve the destination.

`confirmationRequired`

AddMediaMediaDestinationResolutionResult.ConfirmationRequired

A destination that the user must confirm before proceeding.

`disambiguation`

AddMediaMediaDestinationResolutionResult.Disambiguation

Multiple destinations for the user to choose from.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Providing a Destination

object AddMediaMediaDestinationResolutionResult.Success

A media destination that successfully matches an intent.

object MediaDestination

The user’s library or a playlist.

object MediaDestinationLibrary

The user’s library as a destination for an add media intent.

object MediaDestinationPlaylist

A playlist as a destination for an add media intent.

### Reporting a Problem

object AddMediaMediaDestinationResolutionResult.Unsupported

The reason your service can’t add media items to the specified library or playlist.

type AddMediaMediaDestinationUnsupportedReason

Reasons the media service can’t add media items to a specified playlist.

### Clarifying a Possible Match

object AddMediaMediaDestinationResolutionResult.ConfirmationRequired

A result that requires the user to confirm the library or playlist before you add media items to it.

object AddMediaMediaDestinationResolutionResult.Disambiguation

A result that requires the user to choose which library or playlist they want to add media items to.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Identifying a Library or Playlist

object AddMediaIntentHandlingResolveMediaDestinationInvocationResponse

Your service’s response to a request to resolve media items in an add media intent.

