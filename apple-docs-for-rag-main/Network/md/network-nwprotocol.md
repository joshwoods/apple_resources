

- Network
-  NWProtocol 

Class

# NWProtocol

The abstract superclass used by Network framework protocols and by custom network protocols that you define.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NWProtocol
```

## Topics

### Adding Protocols to Connections

class NWProtocolOptions

The abstract superclass for configuring the options of a network protocol.

class NWProtocolDefinition

The abstract superclass for identifying a network protocol.

### Interacting with Protocols

class NWProtocolMetadata

The abstract superclass for specifying metadata about a network protocol.

## Relationships

### Inherited By

- NWProtocolFramer
- NWProtocolIP
- NWProtocolQUIC
- NWProtocolTCP
- NWProtocolTLS
- NWProtocolUDP
- NWProtocolWebSocket

### Conforms To

- Sendable

## See Also

### Modifying Protocol Stacks

var defaultProtocolStack: NWParameters.ProtocolStack

The protocol stack used by connections and listeners.

class ProtocolStack

An ordered set of protocol options that define the protocols that connections and listeners use.

