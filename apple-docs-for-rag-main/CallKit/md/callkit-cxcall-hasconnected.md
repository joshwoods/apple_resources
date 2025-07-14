

- CallKit
- CXCall
-  hasConnected 

Instance Property

# hasConnected

A Boolean value that indicates whether the call has connected.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var hasConnected: Bool { get }
```

## Discussion

A call is considered connected when both caller and callee can start communicating.

## See Also

### Accessing Call Attributes

var uuid: UUID

The unique identifier for the call.

var isOutgoing: Bool

A Boolean value that indicates whether the call is outgoing.

var hasEnded: Bool

A Boolean value that indicates whether the call has ended.

var isOnHold: Bool

A Boolean value that indicates whether the call is on hold.

