

- Foundation
- URLSession
-  webSocketTask(with:) 

Instance Method

# webSocketTask(with:)

Creates a WebSocket task for the provided URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func webSocketTask(with url: URL) -> URLSessionWebSocketTask
```

## Parameters 

`url`  

The WebSocket URL with which to connect.

## Discussion

The provided URL must have a `ws` or `wss` scheme.

## See Also

### Adding WebSocket tasks to a session

func webSocketTask(with: URLRequest) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL request.

func webSocketTask(with: URL, protocols: [String]) -> URLSessionWebSocketTask

Creates a WebSocket task given a URL and an array of protocols.

class URLSessionWebSocketTask

A URL session task that communicates over the WebSockets protocol standard.

protocol URLSessionWebSocketDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to WebSocket tasks.

