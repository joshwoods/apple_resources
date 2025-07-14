

- Foundation
- URLSessionWebSocketTask
-  URLSessionWebSocketTask.Message 

Enumeration

# URLSessionWebSocketTask.Message

An enumeration of the types of messages sent and received.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Message
```

## Topics

### Message types

case data(Data)

A WebSocket message that contains a block of data.

case string(String)

A WebSocket message that contains a string.

## Relationships

### Conforms To

- Sendable

## See Also

### Sending and receiving data

func send(URLSessionWebSocketTask.Message, completionHandler: ((any Error)?) -> Void)

Sends a WebSocket message, receiving the result in a completion handler.

func receive(completionHandler: (Result&lt;URLSessionWebSocketTask.Message, any Error>) -> Void)

Reads a WebSocket message once all the frames of the message are available.

var maximumMessageSize: Int

The maximum number of bytes to buffer before the receive call fails with an error.

