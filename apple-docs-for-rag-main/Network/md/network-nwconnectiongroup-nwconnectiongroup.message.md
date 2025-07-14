

- Network
- NWConnectionGroup
-  NWConnectionGroup.Message 

Class

# NWConnectionGroup.Message

An object that represents a message that you send or receive within a group, and that contains protocol metadata and send properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class Message
```

## Topics

### Inspecting Received Messages

var remoteEndpoint: NWEndpoint?

The endpoint that originates the message you receive.

var localEndpoint: NWEndpoint?

The local address and port you use to receive the message.

var path: NWPath?

The network path on which you receive the message.

### Replying to Received Messages

func reply(content: Data?, message: NWConnectionGroup.Message)

Sends a reply to the specific endpoint that originates a group message you receive.

func extractConnection() -> NWConnection?

Converts a message you receive from an endpoint into a connection object that you use for long-term communication with that endpoint.

### Sending Messages

static let `default`: NWConnectionGroup.Message

A static object you use to send a message with default properties.

init(identifier: String, expiration: UInt64, priority: Double, isFinal: Bool, antecedent: NWConnection.ContentContext?, metadata: [NWProtocolMetadata]?)

Initializes a custom message context you use to send data.

### Initializers

init(nw: nw_content_context_t)

### Instance Methods

func metadata(definition: NWProtocolDefinition) -> NWProtocolMetadata?

## Relationships

### Inherits From

- NWConnection.ContentContext

### Conforms To

- Sendable

## See Also

### Sending and Receiving Group Messages

func setReceiveHandler(maximumMessageSize: Int, rejectOversizedMessages: Bool, handler: ((NWConnectionGroup.Message, Data?, Bool) -> Void)?)

Sets a handler that receives inbound messages from members of the group.

func send(content: Data?, to: NWEndpoint?, message: NWConnectionGroup.Message, completion: (NWError?) -> Void)

Sends data to the entire group, or to a specific member of the group.

