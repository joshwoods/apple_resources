

- Foundation
-  URLSessionWebSocketDelegate 

Protocol

# URLSessionWebSocketDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to WebSocket tasks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol URLSessionWebSocketDelegate : URLSessionTaskDelegate
```

## Topics

### Handling WebSocket lifecycle events

func urlSession(URLSession, webSocketTask: URLSessionWebSocketTask, didOpenWithProtocol: String?)

Tells the delegate that the WebSocket task successfully negotiated the handshake with the endpoint, indicating the negotiated protocol.

func urlSession(URLSession, webSocketTask: URLSessionWebSocketTask, didCloseWith: URLSessionWebSocketTask.CloseCode, reason: Data?)

Tells the delegate that the WebSocket task received a close frame from the server endpoint, optionally including a close code and reason from the server.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate
- URLSessionTaskDelegate

## See Also

### Adding WebSocket tasks to a session

func webSocketTask(with: URL) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL.

func webSocketTask(with: URLRequest) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL request.

func webSocketTask(with: URL, protocols: [String]) -> URLSessionWebSocketTask

Creates a WebSocket task given a URL and an array of protocols.

class URLSessionWebSocketTask

A URL session task that communicates over the WebSockets protocol standard.

