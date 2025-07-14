

- Foundation
- Timer
-  userInfo 

Instance Property

# userInfo

The receiver’s `userInfo` object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: Any? { get }
```

## Discussion

Do not access this property after the timer is invalidated. Use isValid to test whether the timer is valid.

## See Also

### Related Documentation

init(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer object with the specified object and selector.

class func scheduledTimer(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

func invalidate()

Stops the timer from ever firing again and requests its removal from its run loop.

### Retrieving Timer Information

var isValid: Bool

A Boolean value that indicates whether the timer is currently valid.

var fireDate: Date

The date at which the timer will fire.

var timeInterval: TimeInterval

The timer’s time interval, in seconds.

