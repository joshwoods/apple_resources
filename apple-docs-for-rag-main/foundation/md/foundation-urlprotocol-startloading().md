

- Foundation
- URLProtocol
-  startLoading() 

Instance Method

# startLoading()

Starts protocol-specific loading of the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func startLoading()
```

## Discussion

When this method is called, the subclass implementation should start loading the request, providing feedback to the URL loading system via the URLProtocolClient protocol.

Subclasses must implement this method.

## See Also

### Starting and stopping downloads

func stopLoading()

Stops protocol-specific loading of the request.

