

- Foundation
- URLProtocol
-  stopLoading() 

Instance Method

# stopLoading()

Stops protocol-specific loading of the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stopLoading()
```

## Discussion

When this method is called, the subclass implementation should stop loading a request. This could be in response to a cancel operation, so protocol implementations must be able to handle this call while a load is in progress. When your protocol receives a call to this method, it should also stop sending notifications to the client.

Subclasses must implement this method.

## See Also

### Starting and stopping downloads

func startLoading()

Starts protocol-specific loading of the request.

