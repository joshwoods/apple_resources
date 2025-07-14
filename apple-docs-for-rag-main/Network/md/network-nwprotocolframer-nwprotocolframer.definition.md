

- Network
- NWProtocolFramer
-  NWProtocolFramer.Definition 

Class

# NWProtocolFramer.Definition

A custom protocol definition you use to associate messages with protocol options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Definition
```

## Topics

### Defining Framer Protocols

init(implementation: any NWProtocolFramerImplementation.Type)

Initializes a new protocol definition based on your protocol implementation.

## Relationships

### Inherits From

- NWProtocolDefinition

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Using Framers with Connections

class Options

A container you use to add your custom protocol to a connection’s protocol stack.

class Message

A message for a custom protocol, in which you can store arbitrary key-value pairs.

