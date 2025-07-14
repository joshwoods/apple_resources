

- Foundation
- URLSessionWebSocketDelegate
-  urlSession(\_:webSocketTask:didOpenWithProtocol:) 

Instance Method

# urlSession(\_:webSocketTask:didOpenWithProtocol:)

Tells the delegate that the WebSocket task successfully negotiated the handshake with the endpoint, indicating the negotiated protocol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func urlSession(
    _ session: URLSession,
    webSocketTask: URLSessionWebSocketTask,
    didOpenWithProtocol protocol: String?
)
```

## Parameters 

`session`  

The session of the WebSocket task that opened.

`webSocketTask`  

The WebSocket task that opened.

`protocol`  

The protocol picked during the handshake phase. This parameter is `nil` if the server did not pick a protocol, or if the client did not advertise protocols when creating the task.

## Discussion

If the handshake fails, the task doesn’t call this delegate method.

## See Also

### Handling WebSocket lifecycle events

func urlSession(URLSession, webSocketTask: URLSessionWebSocketTask, didCloseWith: URLSessionWebSocketTask.CloseCode, reason: Data?)

Tells the delegate that the WebSocket task received a close frame from the server endpoint, optionally including a close code and reason from the server.

