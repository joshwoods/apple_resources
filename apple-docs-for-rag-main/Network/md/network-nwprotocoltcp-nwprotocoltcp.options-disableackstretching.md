

- Network
- NWProtocolTCP
- NWProtocolTCP.Options
-  disableAckStretching 

Instance Property

# disableAckStretching

A Boolean that disables TCP acknowledgment stretching.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var disableAckStretching: Bool { get set }
```

## See Also

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

var disableECN: Bool

A Boolean that disables negotiation of Explicit Congestion Notification markings.

