

- SiriKit Cloud Media
-  ProtocolExceptionReason 

Type

# ProtocolExceptionReason

Categories of exceptions a service can encounter.

SiriKit Cloud Media 1.0.2+

``` source
string ProtocolExceptionReason
```

## Possible Values 

`unsupported`  

The service doesn’t support this method.

`unauthorized`  

The current user doesn’t have authorization to perform this action.

`unexpected`  

The service receives something unexpected, such as methods for processing an intent in the wrong order.

`invalid`  

The requested method isn’t available on this endpoint.

`unparseable`  

The service can’t parse the request.

`deprecated`  

The current version of the library no longer supports the request.

`internal`  

Something is wrong within the service.

`complex`  

The requested search takes too long to complete.

`busy`  

The service is receiving too many requests. The client uses the `retryWithDelay` value in the ProtocolException to determine when to try again.

## See Also

### Exceptions

object ProtocolExceptionInvocationResponse

A response object that indicates when the service fails to process the client’s request.

object ProtocolException

An exception response from a media service.

