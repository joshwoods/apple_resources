

- Core Telephony
-  CTCall Deprecated

Class

# CTCall

An object used to identify a cellular call and determine its state.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
class CTCall
```

Deprecated

Getting call information in Core Telephony is no longer supported. Use CallKit instead.

## Topics

### Obtaining Information About a Cellular Call

var callID: String

A unique identifier for the cellular call.

var callState: String

The state of the cellular call.

### Getting Cellular Call State

Cellular Call States

States of cellular calls; one of dialing, incoming, connected, or disconnected.

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

class CTCallCenter

An object that provides a list of current cellular calls, and provides the ability to respond to state changes for calls.

Deprecated

