

- Social
- SLRequest
-  perform(handler:) 

Instance Method

# perform(handler:)

Performs an asynchronous request and calls the specified handler when done.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
func perform(handler: SLRequestHandler!)
```

## Parameters 

`handler`  

The handler to call when the request is done. The parameters for this handler are described in SLRequestHandler. This handler is not guaranteed to be called on any particular thread and should not be nil.

## See Also

### Sending a Request

typealias SLRequestHandler

The callback handler for a request.

