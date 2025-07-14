

- Core Telephony
- CTCallCenter
-  currentCalls Deprecated

Instance Property

# currentCalls

An array representing the cellular calls in progress.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var currentCalls: Set? { get }
```

Deprecated

To get a list of active calls, use CXCallObserver in CallKit instead.

## Discussion

An array containing a `CTCall` object for each cellular call in progress. If no calls are in progress, the value of this property is `nil`.

## See Also

### Responding to Cellular Call Events

var callEventHandler: ((CTCall) -> Void)?

A closure dispatched when a call changes state.

Deprecated

