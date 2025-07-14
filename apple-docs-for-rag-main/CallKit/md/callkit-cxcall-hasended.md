

- CallKit
- CXCall
-  hasEnded 

Instance Property

# hasEnded

A Boolean value that indicates whether the call has ended.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var hasEnded: Bool { get }
```

## Discussion

A call is considered ended when the user disconnects or all other callers disconnect.

## See Also

### Accessing Call Attributes

var uuid: UUID

The unique identifier for the call.

var isOutgoing: Bool

A Boolean value that indicates whether the call is outgoing.

var hasConnected: Bool

A Boolean value that indicates whether the call has connected.

var isOnHold: Bool

A Boolean value that indicates whether the call is on hold.

