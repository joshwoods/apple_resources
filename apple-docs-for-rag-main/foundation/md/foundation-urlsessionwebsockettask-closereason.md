

- Foundation
- URLSessionWebSocketTask
-  closeReason 

Instance Property

# closeReason

A block of data that provides further information about why a connection closed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var closeReason: Data? { get }
```

## Discussion

The close reason provides further information about why a connection closed, beyond that provided by the closeCode. The value of this property isn’t defined by RFC 6455; the endpoints define how it’s used.

You can retrieve the close reason at any time. When the task is not yet closed, this value is URLSessionWebSocketTask.CloseCode.invalid.

## See Also

### Closing the connection

func cancel(with: URLSessionWebSocketTask.CloseCode, reason: Data?)

Sends a close frame with the given close code and optional close reason.

var closeCode: URLSessionWebSocketTask.CloseCode

A code that indicates the reason a connection closed.

enum CloseCode

A code that indicates why a WebSocket connection closed.

