

- Network
- NWBrowser
- NWBrowser.Result
-  NWBrowser.Result.Metadata 

Enumeration

# NWBrowser.Result.Metadata

Values associated with discovered services, such as TXT records.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Metadata
```

## Topics

### Metadata Types

case bonjour(NWTXTRecord)

A TXT record associated with a discovered service.

case none

A value indicating that no associated data was discovered on a service.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Evaluating Browser Results

let endpoint: NWEndpoint

The discovered service endpoint.

let interfaces: [NWInterface]

The list of interfaces on which the service was discovered.

let metadata: NWBrowser.Result.Metadata

The metadata associated with the discovered service, such as the TXT record.

struct NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

