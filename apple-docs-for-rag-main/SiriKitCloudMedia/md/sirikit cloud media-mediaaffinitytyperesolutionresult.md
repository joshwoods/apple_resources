

- SiriKit Cloud Media
-  MediaAffinityTypeResolutionResult 

Object

# MediaAffinityTypeResolutionResult

A media affinity that matches an update media affinity intent, or information about why your service can’t determine the media affinity.

SiriKit Cloud Media 1.0.2+

``` source
object MediaAffinityTypeResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `MediaAffinityTypeResolutionResult`

`success`

MediaAffinityTypeResolutionResult.Success

A media affinity that matches the intent.

`confirmationRequired`

MediaAffinityTypeResolutionResult.ConfirmationRequired

A media affinity for the user to confirm or reject before proceeding.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Specifying the Result

object MediaAffinityTypeResolutionResult.ConfirmationRequired

A result that requires the user to confirm the media affinity before proceeding.

object MediaAffinityTypeResolutionResult.Success

A media affinity that successfully matches the intent.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Discerning Like or Dislike

type MediaAffinityType

A preference or dislike for a media item.

object UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse

Your service’s response to a request that expresses a preference or dislike for a media item.

