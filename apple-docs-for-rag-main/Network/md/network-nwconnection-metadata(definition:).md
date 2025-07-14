

- Network
- NWConnection
-  metadata(definition:) 

Instance Method

# metadata(definition:)

Retrieves the connection-wide metadata for a specific protocol.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final func metadata(definition: NWProtocolDefinition) -> NWProtocolMetadata?
```

## See Also

### Inspecting Connections

class NWProtocolMetadata

The abstract superclass for specifying metadata about a network protocol.

let endpoint: NWEndpoint

The remote endpoint with which the connection was initialized.

let parameters: NWParameters

The parameters with which the connection was initialized.

var queue: DispatchQueue?

The queue on which connection events are delivered.

