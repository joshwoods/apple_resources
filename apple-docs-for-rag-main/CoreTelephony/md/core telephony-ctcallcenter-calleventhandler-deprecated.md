

- Core Telephony
- CTCallCenter
-  callEventHandler Deprecated

Instance Property

# callEventHandler

A closure dispatched when a call changes state.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var callEventHandler: ((CTCall) -> Void)? { get set }
```

Deprecated

To monitor state changes in calls, use CXCallObserver in CallKit instead.

## See Also

### Responding to Cellular Call Events

var currentCalls: Set&lt;CTCall>?

An array representing the cellular calls in progress.

Deprecated

