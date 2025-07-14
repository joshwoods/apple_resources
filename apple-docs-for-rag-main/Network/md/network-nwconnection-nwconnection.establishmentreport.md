

- Network
- NWConnection
-  NWConnection.EstablishmentReport 

Structure

# NWConnection.EstablishmentReport

A report that provides metrics about the establishment of a connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct EstablishmentReport
```

## Overview

Use this report to inspect connection establishment details, such as its resolution steps, use of proxies, and duration.

This report shows different data when iCloud Private Relay makes the connection. iCloud Private Relay can change the timing and sequence of events for your connections by using a set of privacy proxies.

When iCloud Private Relay is in use, any proxied connections have the usedProxy property set. The handshakes property contains information about the stages of proxy connections used, and the timings to establish the end-to-end connection.

Connections that aren’t proxied might still use iCloud Private Relay for name resolution. In this case, the resolutions property includes information about resolutions that use the `https` DNS protocol.

## Topics

### Inspecting Connection Attempts

let duration: TimeInterval

The total duration of the successful connection establishment attempt, from the preparing state to the ready state.

let previousAttemptCount: Int

The number of attempts made before the successful attempt, when the connection moved from the preparing state back to the waiting state.

let attemptStartedAfterInterval: TimeInterval

The time between the call to start and the beginning of the successful connection attempt.

### Inspecting Resolution

let resolutions: [NWConnection.EstablishmentReport.Resolution]

The array of resolution steps performed during connection establishment, in order from first resolved to last resolved.

struct Resolution

A description of a single DNS resolution step.

### Inspecting Protocol Handshakes

let handshakes: [NWConnection.EstablishmentReport.Handshake]

The array of protocol handshakes in order from first completed to last completed.

struct Handshake

A description of a single protocol handshake.

### Checking for Proxies

let proxyConfigured: Bool

A Boolean indicating whether a proxy was configured on the connection.

let usedProxy: Bool

A Boolean indicating whether the connection used a proxy.

let proxyEndpoint: NWEndpoint?

The endpoint of the proxy the connection used.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Collecting Connection Metrics

Collecting Network Connection Metrics

Use reports to understand how DNS and protocol handshakes impact connection establishment.

func requestEstablishmentReport(queue: DispatchQueue, completion: (NWConnection.EstablishmentReport?) -> Void)

Requests a copy of the connection’s establishment report once the connection is in the ready state.

func startDataTransferReport() -> NWConnection.PendingDataTransferReport

Begins a new data transfer report, which can later be collected.

class PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

struct DataTransferReport

A report that provides metrics about data being sent and received on a connection.

