

- Network
- NWConnection
-  NWConnection.SendCompletion 

Enumeration

# NWConnection.SendCompletion

A completion handler that indicates when the connection has finished processing sent content.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum SendCompletion
```

## Topics

### Completions

case contentProcessed((NWError?) -> Void)

Provide a completion handler that’s invoked when the sent data is processed by the stack.

case idempotent

Mark the sent data as idempotent—data that can be sent multiple times.

## See Also

### Sending and Receiving Data

func send(content: Data?, contentContext: NWConnection.ContentContext, isComplete: Bool, completion: NWConnection.SendCompletion)

Sends data on a connection.

func send&lt;Content>(content: Content?, contentContext: NWConnection.ContentContext, isComplete: Bool, completion: NWConnection.SendCompletion)

Sends data on a connection using a custom Data type.

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

