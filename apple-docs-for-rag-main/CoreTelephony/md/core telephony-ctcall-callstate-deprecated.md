

- Core Telephony
- CTCall
-  callState Deprecated

Instance Property

# callState

The state of the cellular call.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var callState: String { get }
```

Deprecated

Replaced by \ properties

## Discussion

A cellular call’s initial state is either CTCallStateDialing or CTCallStateIncoming. After establishing the call for all parties involved, the state transitions to CTCallStateConnected. When the call ends, the state transitions to CTCallStateDisconnected.

## See Also

### Obtaining Information About a Cellular Call

var callID: String

A unique identifier for the cellular call.

Deprecated

