

- Network
-  NWProtocolMetadata 

Class

# NWProtocolMetadata

The abstract superclass for specifying metadata about a network protocol.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NWProtocolMetadata
```

## Overview

You can use metadata when sending and receiving messages, as well as when inspecting connection properties.

## Relationships

### Inherited By

- NWProtocolFramer.Message
- NWProtocolIP.Metadata
- NWProtocolQUIC.Metadata
- NWProtocolTCP.Metadata
- NWProtocolTLS.Metadata
- NWProtocolUDP.Metadata
- NWProtocolWebSocket.Metadata

### Conforms To

- Sendable

## See Also

### Inspecting Connections

func metadata(definition: NWProtocolDefinition) -> NWProtocolMetadata?

Retrieves the connection-wide metadata for a specific protocol.

let endpoint: NWEndpoint

The remote endpoint with which the connection was initialized.

let parameters: NWParameters

The parameters with which the connection was initialized.

var queue: DispatchQueue?

The queue on which connection events are delivered.

