

- CallKit
- CXCall
-  isOnHold 

Instance Property

# isOnHold

A Boolean value that indicates whether the call is on hold.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var isOnHold: Bool { get }
```

## Discussion

When a caller places the call on hold, callers are unable to communicate with one another until the holding caller removes the call from hold.

## See Also

### Accessing Call Attributes

var uuid: UUID

The unique identifier for the call.

var isOutgoing: Bool

A Boolean value that indicates whether the call is outgoing.

var hasConnected: Bool

A Boolean value that indicates whether the call has connected.

var hasEnded: Bool

A Boolean value that indicates whether the call has ended.

