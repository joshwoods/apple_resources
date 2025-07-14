

- Network
- NWProtocolFramer
-  NWProtocolFramer.Options 

Class

# NWProtocolFramer.Options

A container you use to add your custom protocol to a connection’s protocol stack.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Options
```

## Topics

### Creating Framer Options

init(definition: NWProtocolFramer.Definition)

Initializes a set of protocol options with a custom framer definition.

### Subscripts

subscript(String) -> Any?

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Using Framers with Connections

class Definition

A custom protocol definition you use to associate messages with protocol options.

class Message

A message for a custom protocol, in which you can store arbitrary key-value pairs.

