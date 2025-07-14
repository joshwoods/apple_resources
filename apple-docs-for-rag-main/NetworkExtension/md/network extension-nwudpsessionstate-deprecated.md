

- Network Extension
-  NWUDPSessionState Deprecated

Enumeration

# NWUDPSessionState

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
enum NWUDPSessionState
```

Deprecated

Use the nw_connection_state_t type from the Network framework instead.

## Topics

### Session States

case invalid

The session is in an invalid or uninitialized state.

case waiting

The session is waiting for better conditions before attempting to make the session ready.

case preparing

The remote endpoint is being resolved.

case ready

The session is ready for reading and writing data.

case failed

None of the currently resolved endpoints can be used at this time, either due to problems with the path or the client rejecting the endpoints.

case cancelled

The session has been cancelled by the client calling `cancel`.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Monitoring the session state

var state: NWUDPSessionState

The current state of the UDP session.

Deprecated

var isViable: Bool

The viability of a UDP session represents whether or not data can be transferred.

Deprecated

