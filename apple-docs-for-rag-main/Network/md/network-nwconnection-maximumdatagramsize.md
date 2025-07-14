

- Network
- NWConnection
-  maximumDatagramSize 

Instance Property

# maximumDatagramSize

The maximum size of a datagram message that can be sent on a connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final var maximumDatagramSize: Int { get }
```

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

func receiveMessage(completion: (Data?, NWConnection.ContentContext?, Bool, NWError?) -> Void)

Schedules a single receive completion handler for a complete message, as opposed to a range of bytes.

func batch(() -> Void)

Defines a block in which calls to send and receive are processed as a batch to improve performance.

class ContentContext

An object that represents a message to send or receive, containing protocol metadata and send properties.

