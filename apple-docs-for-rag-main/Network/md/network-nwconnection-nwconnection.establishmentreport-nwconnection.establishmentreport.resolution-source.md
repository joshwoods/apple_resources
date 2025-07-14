

- Network
- NWConnection
- NWConnection.EstablishmentReport
- NWConnection.EstablishmentReport.Resolution
-  source 

Instance Property

# source

The source of the DNS response.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let source: NWConnection.EstablishmentReport.Resolution.Source
```

## See Also

### Measuring Performance

let duration: TimeInterval

The duration of this resolution step, from when the query was issued to when the response was complete.

enum Source

Sources that may provide DNS responses.

var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol

The transport protocol your connection used for DNS resolution.

enum DNSProtocol

A set of transport protocols connections use for DNS resolution.

