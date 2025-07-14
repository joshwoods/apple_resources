

- Network
- NWConnection
-  receiveMessage(completion:) 

Instance Method

# receiveMessage(completion:)

Schedules a single receive completion handler for a complete message, as opposed to a range of bytes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final func receiveMessage(completion: @escaping (Data?, NWConnection.ContentContext?, Bool, NWError?) -> Void)
```

## Parameters 

`completion`  

A receive completion is invoked exactly once for a call to receive. The completion indicates that the requested content has been received (in which case the content is delivered), or that an error has occurred.

The completion delivers the received content, which may be nil if the message is complete or an error occurred, the message context, a flag indicating if the message is complete, and any associated error.

## Discussion

Receiving messages allows you to deal with complete datagrams or application-layer messages without needing to reconstruct a stream.

If you are using UDP, receiving a message will deliver a single datagram.

If you request to receive a message on a protocol that is otherwise an unbounded bytestream, like TCP or TLS, note that this will not deliver any data until the stream is closed by the peer.

In order to use messages on top of a bytestream protocol, add a protocol such as NWProtocolWebSocket or a custom NWProtocolFramer to your protocol stack.

## See Also

### Sending and Receiving Data

func send(content: Data?, contentContext: NWConnection.ContentContext, isComplete: Bool, completion: NWConnection.SendCompletion)

Sends data on a connection.

func send&lt;Content>(content: Content?, contentContext: NWConnection.ContentContext, isComplete: Bool, completion: NWConnection.SendCompletion)

Sends data on a connection using a custom Data type.

enum SendCompletion

A completion handler that indicates when the connection has finished processing sent content.

func receive(minimumIncompleteLength: Int, maximumLength: Int, completion: (Data?, NWConnection.ContentContext?, Bool, NWError?) -> Void)

Schedules a single receive completion handler, with a range indicating how many bytes the handler can receive at one time.

func batch(() -> Void)

Defines a block in which calls to send and receive are processed as a batch to improve performance.

class ContentContext

An object that represents a message to send or receive, containing protocol metadata and send properties.

var maximumDatagramSize: Int

The maximum size of a datagram message that can be sent on a connection.

