

- Foundation
-  URLSessionWebSocketTask 

Class

# URLSessionWebSocketTask

A URL session task that communicates over the WebSockets protocol standard.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class URLSessionWebSocketTask
```

## Overview

URLSessionWebSocketTask is a concrete subclass of URLSessionTask that provides a message-oriented transport protocol over TCP and TLS in the form of WebSocket framing. It follows the WebSocket Protocol defined in RFC 6455.

You create a URLSessionWebSocketTask with either a `ws:` or `wss:` URL. When creating the task, you can also provide a list of protocols to advertise during the handshake phase. Once the handshake completes, your app receives notifications through the session’s delegate.

You send data with send(_:completionHandler:) and receive data with receive(completionHandler:). The task performs reads and writes asynchronously, and allows you to send and receive messages that contain both binary frames and UTF-8 encoded text frames. The task enqueues any reads or writes you perform prior to the handshake’s completion, and executes them after the handshake completes.

URLSessionWebSocketTask supports redirection and authentication like other types of tasks do, using the methods in URLSessionTaskDelegate. The WebSocket task calls the redirection and authentication delegate methods prior to completing the handshake. The WebSocket task also supports cookies, by storing cookies to the session configuration’s httpCookieStorage, and attaches cookies to outgoing HTTP handshake requests.

Note

watchOS supports URLSessionWebSocketTask for specific use cases. For more details, see TN3135: Low-level networking on watchOS.

## Topics

### Sending and receiving data

func send(URLSessionWebSocketTask.Message, completionHandler: ((any Error)?) -> Void)

Sends a WebSocket message, receiving the result in a completion handler.

enum Message

An enumeration of the types of messages sent and received.

func receive(completionHandler: (Result&lt;URLSessionWebSocketTask.Message, any Error>) -> Void)

Reads a WebSocket message once all the frames of the message are available.

var maximumMessageSize: Int

The maximum number of bytes to buffer before the receive call fails with an error.

### Sending ping frames

func sendPing(pongReceiveHandler: ((any Error)?) -> Void)

Sends a ping frame from the client side, with a closure to receive the pong from the server endpoint.

### Closing the connection

func cancel(with: URLSessionWebSocketTask.CloseCode, reason: Data?)

Sends a close frame with the given close code and optional close reason.

var closeCode: URLSessionWebSocketTask.CloseCode

A code that indicates the reason a connection closed.

enum CloseCode

A code that indicates why a WebSocket connection closed.

var closeReason: Data?

A block of data that provides further information about why a connection closed.

### Instance Methods

func receive() async throws -> URLSessionWebSocketTask.Message

func send(URLSessionWebSocketTask.Message) async throws

## Relationships

### Inherits From

- URLSessionTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- ProgressReporting
- Sendable

## See Also

### Adding WebSocket tasks to a session

func webSocketTask(with: URL) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL.

func webSocketTask(with: URLRequest) -> URLSessionWebSocketTask

Creates a WebSocket task for the provided URL request.

func webSocketTask(with: URL, protocols: [String]) -> URLSessionWebSocketTask

Creates a WebSocket task given a URL and an array of protocols.

protocol URLSessionWebSocketDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to WebSocket tasks.

