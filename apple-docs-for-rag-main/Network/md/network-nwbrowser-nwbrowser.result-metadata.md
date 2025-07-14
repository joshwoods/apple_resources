

- Network
- NWBrowser
- NWBrowser.Result
-  metadata 

Instance Property

# metadata

The metadata associated with the discovered service, such as the TXT record.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let metadata: NWBrowser.Result.Metadata
```

## See Also

### Evaluating Browser Results

let endpoint: NWEndpoint

The discovered service endpoint.

let interfaces: [NWInterface]

The list of interfaces on which the service was discovered.

enum Metadata

Values associated with discovered services, such as TXT records.

struct NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

