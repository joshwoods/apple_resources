

- Network
- NWConnection
- NWConnection.ContentContext
-  expirationMilliseconds 

Instance Property

# expirationMilliseconds

A number of milliseconds after which sending the data associated with this context must begin, otherwise the data is discarded.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final let expirationMilliseconds: UInt64
```

## See Also

### Creating Custom Send Contexts

init(identifier: String, expiration: UInt64, priority: Double, isFinal: Bool, antecedent: NWConnection.ContentContext?, metadata: [NWProtocolMetadata]?)

Initializes a custom message context.

let identifier: String

The identifier of the message, used for debugging.

var protocolMetadata: [NWProtocolMetadata]

An array of protocol metadata used to configure per-message or per-packet properties.

class NWProtocolMetadata

The abstract superclass for specifying metadata about a network protocol.

let antecedent: NWConnection.ContentContext?

An optional message context that must be sent before the context you are sending.

let relativePriority: Double

A relative value of priority used to reorder contexts when sending.

