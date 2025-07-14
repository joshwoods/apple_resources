

- Network
- NWConnection
- NWConnection.EstablishmentReport
-  NWConnection.EstablishmentReport.Resolution 

Structure

# NWConnection.EstablishmentReport.Resolution

A description of a single DNS resolution step.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Resolution
```

## Topics

### Measuring Performance

let duration: TimeInterval

The duration of this resolution step, from when the query was issued to when the response was complete.

let source: NWConnection.EstablishmentReport.Resolution.Source

The source of the DNS response.

enum Source

Sources that may provide DNS responses.

var dnsProtocol: NWConnection.EstablishmentReport.Resolution.DNSProtocol

The transport protocol your connection used for DNS resolution.

enum DNSProtocol

A set of transport protocols connections use for DNS resolution.

### Examining Resolved Endpoints

let successfulEndpoint: NWEndpoint

The resolved endpoint that led to the established connection.

let preferredEndpoint: NWEndpoint

The resolved endpoint that the connection used for its first connection attempt.

let endpointCount: Int

The number of endpoints resolved in this step.

## Relationships

### Conforms To

- Sendable

## See Also

### Inspecting Resolution

let resolutions: [NWConnection.EstablishmentReport.Resolution]

The array of resolution steps performed during connection establishment, in order from first resolved to last resolved.

