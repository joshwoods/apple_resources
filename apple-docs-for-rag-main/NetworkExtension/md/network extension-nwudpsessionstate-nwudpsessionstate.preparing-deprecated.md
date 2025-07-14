

- Network Extension
- NWUDPSessionState
-  NWUDPSessionState.preparing Deprecated

Case

# NWUDPSessionState.preparing

The remote endpoint is being resolved.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
case preparing
```

Deprecated

Use the nw_connection_state_t type from the Network framework instead.

## See Also

### Session States

case invalid

The session is in an invalid or uninitialized state.

Deprecated

case waiting

The session is waiting for better conditions before attempting to make the session ready.

Deprecated

case ready

The session is ready for reading and writing data.

Deprecated

case failed

None of the currently resolved endpoints can be used at this time, either due to problems with the path or the client rejecting the endpoints.

Deprecated

case cancelled

The session has been cancelled by the client calling `cancel`.

Deprecated

