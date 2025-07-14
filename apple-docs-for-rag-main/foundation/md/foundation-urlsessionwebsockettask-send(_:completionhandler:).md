

- Foundation
- URLSessionWebSocketTask
-  send(\_:completionHandler:) 

Instance Method

# send(\_:completionHandler:)

Sends a WebSocket message, receiving the result in a completion handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func send(
    _ message: URLSessionWebSocketTask.Message,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

## Parameters 

`message`  

The WebSocket message to send to the other endpoint.

`completionHandler`  

A closure that receives an NSError that indicates an error encountered while sending, or nil if no error occurred.

## Discussion

If an error occurs while sending the message, any outstanding work also fails.

## See Also

### Sending and receiving data

enum Message

An enumeration of the types of messages sent and received.

func receive(completionHandler: (Result&lt;URLSessionWebSocketTask.Message, any Error>) -> Void)

Reads a WebSocket message once all the frames of the message are available.

var maximumMessageSize: Int

The maximum number of bytes to buffer before the receive call fails with an error.

