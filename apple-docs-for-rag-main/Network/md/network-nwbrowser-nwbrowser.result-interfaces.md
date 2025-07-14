

- Network
- NWBrowser
- NWBrowser.Result
-  interfaces 

Instance Property

# interfaces

The list of interfaces on which the service was discovered.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let interfaces: [NWInterface]
```

## See Also

### Evaluating Browser Results

let endpoint: NWEndpoint

The discovered service endpoint.

let metadata: NWBrowser.Result.Metadata

The metadata associated with the discovered service, such as the TXT record.

enum Metadata

Values associated with discovered services, such as TXT records.

struct NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

