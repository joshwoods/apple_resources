

- Foundation
- Timer
-  init(fireAt:interval:target:selector:userInfo:repeats:) 

Initializer

# init(fireAt:interval:target:selector:userInfo:repeats:)

Initializes a timer using the specified object and selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    fireAt date: Date,
    interval ti: TimeInterval,
    target t: Any,
    selector s: Selector,
    userInfo ui: Any?,
    repeats rep: Bool
)
```

## Parameters 

`date`  

The time at which the timer should first fire.

`ti`  

For a repeating timer, this parameter contains the number of seconds between firings of the timer. If `ti` is less than or equal to `0.0`, this method chooses the nonnegative value of `0.0001` seconds instead.

`t`  

The object to which to send the message specified by `aSelector` when the timer fires. The timer maintains a strong reference to this object until it (the timer) is invalidated.

`s`  

The message to send to `target` when the timer fires.

The selector should have the following signature: `timerFireMethod:` (including a colon to indicate that the method takes an argument). The timer passes itself as the argument, thus the method would adopt the following pattern:

```
- (void)timerFireMethod:(NSTimer *)timer
```

`ui`  

Custom user info for the timer. The timer maintains a strong reference to this object until it (the timer) is invalidated. This parameter may be `nil`.

`rep`  

If true, the timer will repeatedly reschedule itself until invalidated. If false, the timer will be invalidated after it fires.

## Return Value

The receiver, initialized such that, when added to a run loop, it will fire at `date` and then, if `repeats` is true, every `ti` after that.

## Discussion

You must add the new timer to a run loop, using add(_:forMode:). Upon firing, the timer sends the message `aSelector` to `target`. (If the timer is configured to repeat, there is no need to subsequently re-add the timer to the run loop.)

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

init(timeInterval: TimeInterval, invocation: NSInvocation, repeats: Bool)

Initializes a timer object with the specified invocation object.

convenience init(fire: Date, interval: TimeInterval, repeats: Bool, block: (Timer) -> Void)

Initializes a timer for the specified date and time interval with the specified block.

