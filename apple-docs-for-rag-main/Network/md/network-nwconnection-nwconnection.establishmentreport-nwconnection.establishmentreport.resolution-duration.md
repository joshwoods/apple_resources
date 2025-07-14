

- Network
- NWConnection
- NWConnection.EstablishmentReport
- NWConnection.EstablishmentReport.Resolution
-  duration 

Instance Property

# duration

The duration of this resolution step, from when the query was issued to when the response was complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let duration: TimeInterval
```

## See Also

### Measuring Performance

let source: NWConnection.EstablishmentReport.Resolution.Source

The source of the DNS response.

enum Source

Sources that may provide DNS responses.

var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol

The transport protocol your connection used for DNS resolution.

enum DNSProtocol

A set of transport protocols connections use for DNS resolution.

