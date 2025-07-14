

- Network
- NWConnection
- NWConnection.EstablishmentReport
- NWConnection.EstablishmentReport.Resolution
-  NWConnection.EstablishmentReport.Resolution.Source 

Enumeration

# NWConnection.EstablishmentReport.Resolution.Source

Sources that may provide DNS responses.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Source
```

## Topics

### Resolution Sources

case query

The DNS response was received from the network.

case cache

The DNS response was retrieved from a local cache.

case expiredCache

The DNS response had expired and was retrieved from a local cache.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Measuring Performance

let duration: TimeInterval

The duration of this resolution step, from when the query was issued to when the response was complete.

let source: NWConnection.EstablishmentReport.Resolution.Source

The source of the DNS response.

var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol

The transport protocol your connection used for DNS resolution.

enum DNSProtocol

A set of transport protocols connections use for DNS resolution.

