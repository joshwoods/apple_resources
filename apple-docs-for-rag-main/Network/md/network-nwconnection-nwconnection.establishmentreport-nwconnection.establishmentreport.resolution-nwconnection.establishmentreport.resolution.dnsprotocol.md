

- Network
- NWConnection
- NWConnection.EstablishmentReport
- NWConnection.EstablishmentReport.Resolution
-  NWConnection.EstablishmentReport.Resolution.DNSProtocol 

Enumeration

# NWConnection.EstablishmentReport.Resolution.DNSProtocol

A set of transport protocols connections use for DNS resolution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum DNSProtocol
```

## Topics

### Resolution Transports

case unknown

The DNS response protocol is unknown or not applicable.

case udp

The connection used cleartext UDP for DNS resolution.

case tcp

The connection used cleartext TCP for DNS resolution.

case tls

The connection used TLS for DNS resolution.

case https

The connection used HTTPS for DNS resolution.

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

enum Source

Sources that may provide DNS responses.

var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol

The transport protocol your connection used for DNS resolution.

