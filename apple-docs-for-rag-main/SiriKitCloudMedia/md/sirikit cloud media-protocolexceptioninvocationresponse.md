

- SiriKit Cloud Media
-  ProtocolExceptionInvocationResponse 

Object

# ProtocolExceptionInvocationResponse

A response object that indicates when the service fails to process the client’s request.

SiriKit Cloud Media 1.0.2+

``` source
object ProtocolExceptionInvocationResponse
```

## Properties

`exception`

ProtocolException

 (Required) 

The reason your service can’t provide a response.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `ProtocolException`

## Discussion

When your service receives a well-formed request, but it can’t fulfill the intent, use an IntentResponse or IntentResolutionResult instead of a `ProtocolExceptionInvocationResponse`. Those objects allow the client to provide more specific information to the user about errors that occur.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Exceptions

object ProtocolException

An exception response from a media service.

type ProtocolExceptionReason

Categories of exceptions a service can encounter.

