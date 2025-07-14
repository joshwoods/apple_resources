

- Network Extension
- NWUDPSession
-  isViable Deprecated

Instance Property

# isViable

The viability of a UDP session represents whether or not data can be transferred.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var isViable: Bool { get }
```

Deprecated

Use the nw_connection_set_viability_changed_handler(_:_:) function from the Network framework instead.

## Discussion

Evaluates to true if the session can read and write data, false otherwise. Use Key-Value Observing to watch this property.

## See Also

### Monitoring the session state

var state: NWUDPSessionState

The current state of the UDP session.

Deprecated

enum NWUDPSessionStateDeprecated

