

- Foundation
- URLSessionWebSocketTask
-  cancel(with:reason:) 

Instance Method

# cancel(with:reason:)

Sends a close frame with the given close code and optional close reason.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func cancel(
    with closeCode: URLSessionWebSocketTask.CloseCode,
    reason: Data?
)
```

## Parameters 

`closeCode`  

A URLSessionWebSocketTask.CloseCode that indicates the reason for closing the connection.

`reason`  

Optional further information to explain the closing. The value of this parameter is defined by the endpoints, not by the standard.

## Discussion

If you call cancel() on the task instead of this method, it sends a cancellation frame with no close code or reason.

## See Also

### Closing the connection

var closeCode: URLSessionWebSocketTask.CloseCode

A code that indicates the reason a connection closed.

enum CloseCode

A code that indicates why a WebSocket connection closed.

var closeReason: Data?

A block of data that provides further information about why a connection closed.

