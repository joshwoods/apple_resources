

- Foundation
- URLSessionWebSocketTask
-  maximumMessageSize 

Instance Property

# maximumMessageSize

The maximum number of bytes to buffer before the receive call fails with an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var maximumMessageSize: Int { get set }
```

## Discussion

This value includes the sum of all bytes from continuation frames. Receive calls will fail once the task reaches this limit.

## See Also

### Sending and receiving data

func send(URLSessionWebSocketTask.Message, completionHandler: ((any Error)?) -> Void)

Sends a WebSocket message, receiving the result in a completion handler.

enum Message

An enumeration of the types of messages sent and received.

func receive(completionHandler: (Result&lt;URLSessionWebSocketTask.Message, any Error>) -> Void)

Reads a WebSocket message once all the frames of the message are available.

