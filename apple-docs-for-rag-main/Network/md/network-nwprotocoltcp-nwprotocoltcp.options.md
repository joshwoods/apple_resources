

- Network
- NWProtocolTCP
-  NWProtocolTCP.Options 

Class

# NWProtocolTCP.Options

A container of options for configuring how TCP is used on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Options
```

## Topics

### Customizing TCP Options

init()

Initializes a default set of TCP connection options.

var enableFastOpen: Bool

A Boolean that enables TCP Fast Open on a connection.

var maximumSegmentSize: Int

TCP’s maximum segment size in bytes.

var noDelay: Bool

A Boolean that disables Nagle’s algorithm for TCP.

var noOptions: Bool

A Boolean that sets TCP into no-options mode.

var noPush: Bool

A Boolean that sets TCP into no-push mode.

var retransmitFinDrop: Bool

A Boolean that causes TCP to drop its connection after not receiving an ACK packet after a FIN packet.

var disableAckStretching: Bool

A Boolean that disables TCP acknowledgment stretching.

var disableECN: Bool

A Boolean that disables negotiation of Explicit Congestion Notification markings.

### Configuring Keepalives

var enableKeepalive: Bool

A Boolean that enables TCP keepalives.

var keepaliveIdle: Int

The number of seconds of idleness that TCP waits before sending keepalive probes.

var keepaliveCount: Int

The number of keepalive probes that TCP sends before terminating the connection.

var keepaliveInterval: Int

The number of seconds that TCP waits between sending keepalive probes.

### Setting Timeouts

var connectionTimeout: Int

The number of seconds that TCP waits before timing out its handshake.

var connectionDropTime: Int

The timeout, in seconds, for TCP retransmission attempts.

var persistTimeout: Int

The TCP persist timeout, in seconds, as defined by RFC 6429.

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Creating TCP Connections

static let definition: NWProtocolDefinition

The system definition of the Transport Control Protocol.

