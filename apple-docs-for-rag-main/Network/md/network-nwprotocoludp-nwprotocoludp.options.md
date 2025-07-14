

- Network
- NWProtocolUDP
-  NWProtocolUDP.Options 

Class

# NWProtocolUDP.Options

A container of options for configuring how UDP is used on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Options
```

## Topics

### Customizing UDP Connections

init()

Initializes a default set of UDP connection options.

var preferNoChecksum: Bool

A Boolean that configures the connection to not send UDP checksums.

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Creating UDP Connections

static let definition: NWProtocolDefinition

The system definition of the User Datagram Protocol.

