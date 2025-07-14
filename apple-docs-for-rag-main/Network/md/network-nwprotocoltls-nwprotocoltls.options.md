

- Network
- NWProtocolTLS
-  NWProtocolTLS.Options 

Class

# NWProtocolTLS.Options

A container of options for configuring how TLS is used on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Options
```

## Topics

### Customizing TLS Connections

init()

Initializes a default set of TLS connection options.

var securityProtocolOptions: sec_protocol_options_t

The handshake security options TLS uses.

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Creating TLS Connections

static let definition: NWProtocolDefinition

The system definition of the Transport Layer Security protocol.

