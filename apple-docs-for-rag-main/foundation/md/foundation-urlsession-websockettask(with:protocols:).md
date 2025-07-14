

- Foundation
- URLSession
-  webSocketTask(with:protocols:) 

Instance Method

# webSocketTask(with:protocols:)

Creates a WebSocket task given a URL and an array of protocols.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func webSocketTask(
    with url: URL,
    protocols: [String]
) -> URLSessionWebSocketTask
```

## Parameters 

`url`  

The WebSocket URL with which to connect.

`protocols`  

An array of protocols to negotiate with the server.

## Discussion

During the WebSocket handshake, the task uses the provided protocols to negotiate a preferred protocol with the server.

Note

The protocol doesn’t affect the WebSocket framing. More details on the protocol are available in RFC 6455, The WebSocket Protocol.

## See Also

### Adding WebSocket tasks to a session

func webSocketTask(with: URL) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL.

func webSocketTask(with: URLRequest) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL request.

class URLSessionWebSocketTask

A URL session task that communicates over the WebSockets protocol standard.

protocol URLSessionWebSocketDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to WebSocket tasks.

