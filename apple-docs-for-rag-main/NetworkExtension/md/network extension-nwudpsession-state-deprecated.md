

- Network Extension
- NWUDPSession
-  state Deprecated

Instance Property

# state

The current state of the UDP session.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var state: NWUDPSessionState { get }
```

Deprecated

Use the nw_connection_set_state_changed_handler(_:_:) function from the Network framework instead.

## Discussion

Use Key-Value Observing (KVO) to monitor the state. If the state is `NWUDPSessionStateReady`, then the connection is eligible for reading and writing. The state will be `NWUDPSessionStateFailed` if the endpoint could not be resolved, or all endpoints have been rejected. For information about KVO, see Key-Value Observing Programming Guide.

## See Also

### Monitoring the session state

enum NWUDPSessionStateDeprecated

var isViable: Bool

The viability of a UDP session represents whether or not data can be transferred.

Deprecated

