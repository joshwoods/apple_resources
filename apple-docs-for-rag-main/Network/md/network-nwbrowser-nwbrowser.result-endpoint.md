

- Network
- NWBrowser
- NWBrowser.Result
-  endpoint 

Instance Property

# endpoint

The discovered service endpoint.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let endpoint: NWEndpoint
```

## See Also

### Evaluating Browser Results

let interfaces: [NWInterface]

The list of interfaces on which the service was discovered.

let metadata: NWBrowser.Result.Metadata

The metadata associated with the discovered service, such as the TXT record.

enum Metadata

Values associated with discovered services, such as TXT records.

struct NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

