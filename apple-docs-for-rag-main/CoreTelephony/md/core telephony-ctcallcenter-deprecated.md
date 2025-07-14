

- Core Telephony
-  CTCallCenter Deprecated

Class

# CTCallCenter

An object that provides a list of current cellular calls, and provides the ability to respond to state changes for calls.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class CTCallCenter
```

Deprecated

Getting call information in Core Telephony is no longer supported. Use CallKit instead.

## Topics

### Responding to Cellular Call Events

var callEventHandler: ((CTCall) -> Void)?

A closure dispatched when a call changes state.

var currentCalls: Set&lt;CTCall>?

An array representing the cellular calls in progress.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Call Information

class CTCall

An object used to identify a cellular call and determine its state.

Deprecated

