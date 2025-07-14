

- Foundation
- URLSessionWebSocketTask
- URLSessionWebSocketTask.Message
-  URLSessionWebSocketTask.Message.string(\_:) 

Case

# URLSessionWebSocketTask.Message.string(\_:)

A WebSocket message that contains a string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case string(String)
```

## Discussion

The URLSessionWebSocketTask uses UTF-8 encoding to send the message’s string.

## See Also

### Message types

case data(Data)

A WebSocket message that contains a block of data.

