

- Foundation
- Timer
-  timeInterval 

Instance Property

# timeInterval

The timer’s time interval, in seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeInterval: TimeInterval { get }
```

## Discussion

If the timer is non-repeating, returns `0` even if a time interval was set.

## See Also

### Retrieving Timer Information

var isValid: Bool

A Boolean value that indicates whether the timer is currently valid.

var fireDate: Date

The date at which the timer will fire.

var userInfo: Any?

The receiver’s `userInfo` object.

