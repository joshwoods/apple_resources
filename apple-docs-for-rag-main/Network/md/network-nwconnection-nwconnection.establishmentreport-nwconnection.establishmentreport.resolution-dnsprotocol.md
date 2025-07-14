

- Network
- NWConnection
- NWConnection.EstablishmentReport
- NWConnection.EstablishmentReport.Resolution
-  dnsProtocol 

Instance Property

# dnsProtocol

The transport protocol your connection used for DNS resolution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol { get }
```

## See Also

### Measuring Performance

let duration: TimeInterval

The duration of this resolution step, from when the query was issued to when the response was complete.

let source: NWConnection.EstablishmentReport.Resolution.Source

The source of the DNS response.

enum Source

Sources that may provide DNS responses.

enum DNSProtocol

A set of transport protocols connections use for DNS resolution.

