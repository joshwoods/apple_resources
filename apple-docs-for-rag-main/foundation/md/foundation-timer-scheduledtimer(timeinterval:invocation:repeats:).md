

- Foundation
- Timer
-  scheduledTimer(timeInterval:invocation:repeats:) 

Type Method

# scheduledTimer(timeInterval:invocation:repeats:)

Creates a new timer and schedules it on the current run loop in the default mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func scheduledTimer(
    timeInterval ti: TimeInterval,
    invocation: NSInvocation,
    repeats yesOrNo: Bool
) -> Timer
```

## Parameters 

`ti`  

The number of seconds between firings of the timer. If `ti` is less than or equal to `0.0`, this method chooses the nonnegative value of `0.0001` seconds instead.

`invocation`  

The invocation to use when the timer fires. The invocation object maintains a strong reference to its arguments until the timer is invalidated.

`yesOrNo`  

If true, the timer will repeatedly reschedule itself until invalidated. If false, the timer will be invalidated after it fires.

## Return Value

A new `NSTimer` object, configured according to the specified parameters.

## Discussion

After `ti` seconds have elapsed, the timer fires, invoking `invocation`.

## See Also

### Related Documentation

Threading Programming Guide

Timer Programming Topics

### Creating a Timer

class func scheduledTimer(withTimeInterval: TimeInterval, repeats: Bool, block: (Timer) -> Void) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

class func scheduledTimer(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

init(timeInterval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer object with the specified time interval and block.

init(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer object with the specified object and selector.

init(timeInterval: TimeInterval, invocation: NSInvocation, repeats: Bool)

Initializes a timer object with the specified invocation object.

convenience init(fire: Date, interval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer for the specified date and time interval with the specified block.

init(fireAt: Date, interval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer using the specified object and selector.

