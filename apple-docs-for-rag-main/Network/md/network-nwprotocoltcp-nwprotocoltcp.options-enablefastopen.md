

- Network
- NWProtocolTCP
- NWProtocolTCP.Options
-  enableFastOpen 

Instance Property

# enableFastOpen

A Boolean that enables TCP Fast Open on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var enableFastOpen: Bool { get set }
```

## Discussion

If TCP Fast Open is enabled and TLS is running on top of TCP, the TLS handshake will automatically be used as the TCP early data. If there is no protocol running on top of TCP, you should also enable fast open on the connection parameters and send idempotent data.

## See Also

### Related Documentation

var allowFastOpen: Bool

A Boolean that enables sending application data with protocol handshakes.

case idempotent

Mark the sent data as idempotent—data that can be sent multiple times.

### Customizing TCP Options

init()

Initializes a default set of TCP connection options.

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

