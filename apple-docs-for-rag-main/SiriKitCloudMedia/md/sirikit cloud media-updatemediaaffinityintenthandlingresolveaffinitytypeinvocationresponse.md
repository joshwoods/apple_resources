

- SiriKit Cloud Media
-  UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse 

Object

# UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse

Your service’s response to a request that expresses a preference or dislike for a media item.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse
```

## Properties

`result`

UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `UpdateMediaAffinityIntentHandling.resolveAffinityType`

## Topics

### Specifying the Result

object UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse.Result

The results of resolving the media affinity in an update media affinity intent.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Discerning Like or Dislike

type MediaAffinityType

A preference or dislike for a media item.

object MediaAffinityTypeResolutionResult

A media affinity that matches an update media affinity intent, or information about why your service can’t determine the media affinity.

