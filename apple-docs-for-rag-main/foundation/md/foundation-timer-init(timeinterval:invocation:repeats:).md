

- Foundation
- Timer
-  init(timeInterval:invocation:repeats:) 

Initializer

# init(timeInterval:invocation:repeats:)

Initializes a timer object with the specified invocation object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    timeInterval ti: TimeInterval,
    invocation: NSInvocation,
    repeats yesOrNo: Bool
)
```

## Parameters 

`ti`  

The number of seconds between firings of the timer. If `ti` is less than or equal to `0.0`, this method chooses the nonnegative value of `0.0001` seconds instead.

`invocation`  

The invocation to use when the timer fires. The timer instructs the invocation object to maintain a strong reference to its arguments.

`yesOrNo`  

If true, the timer will repeatedly reschedule itself until invalidated. If false, the timer will be invalidated after it fires.

## Return Value

A new `NSTimer` object, configured according to the specified parameters.

## Discussion

You must add the new timer to a run loop, using add(_:forMode:). Then, after `ti` have elapsed, the timer fires, invoking `invocation`. (If the timer is configured to repeat, there is no need to subsequently re-add the timer to the run loop.)

## See Also

### Creating a Timer

class func scheduledTimer(withTimeInterval: TimeInterval, repeats: Bool, block: (Timer) -> Void) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

class func scheduledTimer(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

class func scheduledTimer(timeInterval: TimeInterval, invocation: NSInvocation, repeats: Bool) -> Timer

Creates a new timer and schedules it on the current run loop in the default mode.

init(timeInterval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer object with the specified time interval and block.

init(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer object with the specified object and selector.

convenience init(fire: Date, interval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer for the specified date and time interval with the specified block.

init(fireAt: Date, interval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer using the specified object and selector.

