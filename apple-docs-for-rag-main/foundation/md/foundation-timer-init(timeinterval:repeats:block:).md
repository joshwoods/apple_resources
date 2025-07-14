

- Foundation
- Timer
-  init(timeInterval:repeats:block:) 

Initializer

# init(timeInterval:repeats:block:)

Initializes a timer object with the specified time interval and block.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    timeInterval interval: TimeInterval,
    repeats: Bool,
    block: @escaping (Timer) -> Void
)
```

## Parameters 

`interval`  

The number of seconds between firings of the timer. If `interval` is less than or equal to `0.0`, this method chooses the nonnegative value of `0.0001` seconds instead.

`repeats`  

If `true`, the timer will repeatedly reschedule itself until invalidated. If `false`, the timer will be invalidated after it fires.

`block`  

A block to be executed when the timer fires. The block takes a single Timer parameter and has no return value.

## Return Value

A new Timer object, configured according to the specified parameters.

## Discussion

You must add the new timer to a run loop, using add(_:forMode:). Then, after `interval` seconds have elapsed, the timer fires, executing `block`. (If the timer is configured to repeat, you don’t need to add the timer to the run loop again.)

## See Also

### Creating a Timer

class func scheduledTimer(withTimeInterval: TimeInterval, repeats: Bool, block: (Timer) -> Void) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

class func scheduledTimer(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool) -> Timer

Creates a timer and schedules it on the current run loop in the default mode.

class func scheduledTimer(timeInterval: TimeInterval, invocation: NSInvocation, repeats: Bool) -> Timer

Creates a new timer and schedules it on the current run loop in the default mode.

init(timeInterval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer object with the specified object and selector.

init(timeInterval: TimeInterval, invocation: NSInvocation, repeats: Bool)

Initializes a timer object with the specified invocation object.

convenience init(fire: Date, interval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer for the specified date and time interval with the specified block.

init(fireAt: Date, interval: TimeInterval, target: Any, selector: Selector, userInfo: Any?, repeats: Bool)

Initializes a timer using the specified object and selector.

