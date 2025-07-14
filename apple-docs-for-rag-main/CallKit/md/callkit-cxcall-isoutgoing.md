

- CallKit
- CXCall
-  isOutgoing 

Instance Property

# isOutgoing

A Boolean value that indicates whether the call is outgoing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var isOutgoing: Bool { get }
```

## Discussion

An outgoing call is a call initiated by the user, as opposed to an incoming call which is received by the telephony provider.

## See Also

### Accessing Call Attributes

var uuid: UUID

The unique identifier for the call.

var hasConnected: Bool

A Boolean value that indicates whether the call has connected.

var hasEnded: Bool

A Boolean value that indicates whether the call has ended.

var isOnHold: Bool

A Boolean value that indicates whether the call is on hold.

