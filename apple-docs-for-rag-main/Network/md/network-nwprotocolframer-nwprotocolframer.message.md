

- Network
- NWProtocolFramer
-  NWProtocolFramer.Message 

Class

# NWProtocolFramer.Message

A message for a custom protocol, in which you can store arbitrary key-value pairs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Message
```

## Topics

### Creating Framer Messages

init(definition: NWProtocolFramer.Definition)

Initializes an empty message for a custom framer definition.

init(instance: NWProtocolFramer.Instance)

Initializes an empty message from within a framer implementation.

### Accessing Message Metadata

subscript(String) -> Any?

Get and set object values in a custom framer message.

## Relationships

### Inherits From

- NWProtocolMetadata

### Conforms To

- Sendable

## See Also

### Using Framers with Connections

class Definition

A custom protocol definition you use to associate messages with protocol options.

class Options

A container you use to add your custom protocol to a connection’s protocol stack.

