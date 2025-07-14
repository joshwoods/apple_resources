

- Foundation
- Timer
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether the timer is currently valid.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isValid: Bool { get }
```

## Discussion

true if the receiver is still capable of firing or false if the timer has been invalidated and is no longer capable of firing.

## See Also

### Retrieving Timer Information

var fireDate: Date

The date at which the timer will fire.

var timeInterval: TimeInterval

The timer’s time interval, in seconds.

var userInfo: Any?

The receiver’s `userInfo` object.

