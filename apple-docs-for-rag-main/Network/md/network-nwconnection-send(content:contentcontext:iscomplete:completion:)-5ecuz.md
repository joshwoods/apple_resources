

- Network
- NWConnection
-  send(content:contentContext:isComplete:completion:) 

Instance Method

# send(content:contentContext:isComplete:completion:)

Sends data on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final func send(
    content: Data?,
    contentContext: NWConnection.ContentContext = .defaultMessage,
    isComplete: Bool = true,
    completion: NWConnection.SendCompletion
)
```

## Parameters 

`content`  

The data to send on the connection. May be nil if this send marks its context as complete, such as by sending finalMessage as the context and marking the send complete to send a write-close.

`contentContext`  

The context associated with the content, which represents a logical message to be sent on the connection. All content sent within a single context will be sent as an in-order unit, up until the point that the context is marked complete. Once a context is marked complete, it may be re-used as a new logical message. Protocols like TCP that cannot send multiple independent messages at once (serial bytestreams) will only start processing a new context once the prior context has been marked complete. Defaults to defaultMessage.

`isComplete`  

A flag indicating if the caller’s sending context (logical message) is now complete. Until a context is marked complete, content sent for other contexts may not be sent immediately (if the protocol requires sending bytes serially, like TCP). For datagram protocols, like UDP, this flag indicates that the content represents a complete datagram.

When sending using streaming protocols like TCP, this flag can be used to mark the end of a single message on the stream, of which there may be many. However, it can also indicate that the connection should send a “write close” (a TCP FIN) if the sending context is the final context on the connection. Specifically, to send a “write close”, pass finalMessage or defaultStream for the context (or create a custom context and set isFinal), and mark the send as complete.

`completion`  

A completion handler (NWConnection.SendCompletion.contentProcessed(_:)) to notify the caller when content has been processed by the connection, or a marker that this data is idempotent (NWConnection.SendCompletion.idempotent) and may be sent multiple times as fast open data if allowFastOpen is set.

## See Also

### Sending and Receiving Data

func send&lt;Content>(content: Content?, contentContext: NWConnection.ContentContext, isComplete: Bool, completion: NWConnection.SendCompletion)

Sends data on a connection using a custom Data type.

enum SendCompletion

A completion handler that indicates when the connection has finished processing sent content.

func receive(minimumIncompleteLength: Int, maximumLength: Int, completion: (Data?, NWConnection.ContentContext?, Bool, NWError?) -> Void)

Schedules a single receive completion handler, with a range indicating how many bytes the handler can receive at one time.

func receiveMessage(completion: (Data?, NWConnection.ContentContext?, Bool, NWError?) -> Void)

Schedules a single receive completion handler for a complete message, as opposed to a range of bytes.

func batch(() -> Void)

Defines a block in which calls to send and receive are processed as a batch to improve performance.

class ContentContext

An object that represents a message to send or receive, containing protocol metadata and send properties.

var maximumDatagramSize: Int

The maximum size of a datagram message that can be sent on a connection.

