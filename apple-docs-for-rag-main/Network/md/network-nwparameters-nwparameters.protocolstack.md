

- Network
- NWParameters
-  NWParameters.ProtocolStack 

Class

# NWParameters.ProtocolStack

An ordered set of protocol options that define the protocols that connections and listeners use.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class ProtocolStack
```

## Topics

### Adding Application Protocols

var applicationProtocols: [NWProtocolOptions]

The array of application protocol options used by connections and listeners.

### Configuring Lower Protocols

var transportProtocol: NWProtocolOptions?

The transport protocol options used by connections and listeners.

var internetProtocol: NWProtocolOptions?

The Internet Protocol options used by connections and listeners.

## Relationships

### Conforms To

- Sendable

## See Also

### Modifying Protocol Stacks

var defaultProtocolStack: NWParameters.ProtocolStack

The protocol stack used by connections and listeners.

class NWProtocol

The abstract superclass used by Network framework protocols and by custom network protocols that you define.

