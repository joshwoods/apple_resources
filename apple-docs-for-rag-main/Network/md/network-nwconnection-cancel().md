

- Network
- NWConnection
-  cancel() 

Instance Method

# cancel()

Cancels the connection and gracefully disconnects any established network protocols.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final func cancel()
```

## See Also

### Canceling Connections

func forceCancel()

Cancels the connection and immediately disconnects any established network protocols.

func cancelCurrentEndpoint()

Causes the current endpoint to be rejected, allowing the connection to try another resolved address.

