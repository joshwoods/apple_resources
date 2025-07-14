

- Network
- NWConnection
-  NWConnection.ContentContext 

Class

# NWConnection.ContentContext

An object that represents a message to send or receive, containing protocol metadata and send properties.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class ContentContext
```

## Overview

For sending, you should use defaultMessage unless there is a reason to override some values.

You can pass finalMessage to mark the final message in a connection. Once this context is used for sending, and the send is marked as complete, no more data can be sent on the connection.

If you are using a protocol that expects message content, like WebSocket or a custom framer, create a custom context and set metadata using protocolMetadata.

## Topics

### Using Constant Send Contexts

static let defaultMessage: NWConnection.ContentContext

A static context representing a message with default properties.

static let finalMessage: NWConnection.ContentContext

A static context that’s marked as the final message in a connection.

static let defaultStream: NWConnection.ContentContext

A static context representing the total stream of bytes on a connection.

### Creating Custom Send Contexts

init(identifier: String, expiration: UInt64, priority: Double, isFinal: Bool, antecedent: NWConnection.ContentContext?, metadata: [NWProtocolMetadata]?)

Initializes a custom message context.

let identifier: String

The identifier of the message, used for debugging.

var protocolMetadata: [NWProtocolMetadata]

An array of protocol metadata used to configure per-message or per-packet properties.

class NWProtocolMetadata

The abstract superclass for specifying metadata about a network protocol.

let antecedent: NWConnection.ContentContext?

An optional message context that must be sent before the context you are sending.

let expirationMilliseconds: UInt64

A number of milliseconds after which sending the data associated with this context must begin, otherwise the data is discarded.

let relativePriority: Double

A relative value of priority used to reorder contexts when sending.

### Inspecting Receive Contexts

let isFinal: Bool

A Boolean indicating whether this context represents the final message being sent or received.

func protocolMetadata(definition: NWProtocolDefinition) -> NWProtocolMetadata?

Retreives the metadata associated with a specific protocol.

## Relationships

### Inherited By

- NWConnectionGroup.Message

### Conforms To

- Sendable

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

var maximumDatagramSize: Int

The maximum size of a datagram message that can be sent on a connection.

