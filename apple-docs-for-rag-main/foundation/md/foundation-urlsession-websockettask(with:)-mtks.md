

- Foundation
- URLSession
-  webSocketTask(with:) 

Instance Method

# webSocketTask(with:)

Creates a WebSocket task for the provided URL request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func webSocketTask(with request: URLRequest) -> URLSessionWebSocketTask
```

## Parameters 

`request`  

A URL request that indicates a WebSockets endpoint with which to connect.

## Discussion

You can modify the request’s properties prior to calling resume() on the task. The task uses these properties during the HTTP handshake phase.

To add custom protocols, add a header with the key `Sec-WebSocket-Protocol`, and a comma-separated list of protocols you want to negotiate with the server. The custom HTTP headers provided by the client remain unchanged for the handshake with the server.

## See Also

### Adding WebSocket tasks to a session

func webSocketTask(with: URL) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL.

func webSocketTask(with: URL, protocols: [String]) -> URLSessionWebSocketTask

Creates a WebSocket task given a URL and an array of protocols.

class URLSessionWebSocketTask

A URL session task that communicates over the WebSockets protocol standard.

protocol URLSessionWebSocketDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to WebSocket tasks.

