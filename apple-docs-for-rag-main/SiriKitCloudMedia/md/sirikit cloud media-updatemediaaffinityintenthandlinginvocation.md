

- SiriKit Cloud Media
-  UpdateMediaAffinityIntentHandlingInvocation 

Object

# UpdateMediaAffinityIntentHandlingInvocation

A request to process an update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntentHandlingInvocation
```

## Properties

`params`

UpdateMediaAffinityIntentHandlingInvocation.Params

 (Required) 

The parameters of this request, including the update media affinity intent.

`method`

`string`

 (Required) 

The action for your service to take to process this intent.

Possible Values: `UpdateMediaAffinityIntentHandling.resolveMediaItems, UpdateMediaAffinityIntentHandling.resolveAffinityType, UpdateMediaAffinityIntentHandling.handle`

## Topics

### Accessing the Intent

object UpdateMediaAffinityIntentHandlingInvocation.Params

The parameters of an update media affinity intent request.

## Relationships

### Inherits From

- Invocation

## See Also

### Processing an Update Media Affinity Intent

object UpdateMediaAffinityIntent

An object that describes a user’s stated preference regarding media items.

type UpdateMediaAffinityIntentHandlingInvocationResponse

The service’s response to a request to process an update media affinity intent.

