

- SiriKit Cloud Media
-  AddMediaIntentHandlingInvocation 

Object

# AddMediaIntentHandlingInvocation

A request to process an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentHandlingInvocation
```

## Properties

`params`

AddMediaIntentHandlingInvocation.Params

 (Required) 

The parameters of this request, including the add media intent.

`method`

`string`

 (Required) 

An action for your service to take to process this intent.

Possible Values: `AddMediaIntentHandling.resolveMediaItems, AddMediaIntentHandling.resolveMediaDestination, AddMediaIntentHandling.confirm, AddMediaIntentHandling.handle`

## Topics

### Accessing the Intent

object AddMediaIntentHandlingInvocation.Params

The parameters of an add media intent request.

## Relationships

### Inherits From

- Invocation

## See Also

### Processing an Add Media Intent

object AddMediaIntent

An object that describes the user’s request to add media items to their library or to a specific playlist.

type AddMediaIntentHandlingInvocationResponse

The service’s response to a request to process an add media intent.

