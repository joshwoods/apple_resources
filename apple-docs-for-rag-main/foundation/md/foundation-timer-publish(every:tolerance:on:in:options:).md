

- Foundation
- Timer
-  publish(every:tolerance:on:in:options:) 

Type Method

# publish(every:tolerance:on:in:options:)

Returns a publisher that repeatedly emits the current date on the given interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func publish(
    every interval: TimeInterval,
    tolerance: TimeInterval? = nil,
    on runLoop: RunLoop,
    in mode: RunLoop.Mode,
    options: RunLoop.SchedulerOptions? = nil
) -> Timer.TimerPublisher
```

## Parameters 

`interval`  

The time interval on which to publish events. For example, a value of `0.5` publishes an event approximately every half-second.

`tolerance`  

The allowed timing variance when emitting events. Defaults to `nil`, which allows any variance.

`runLoop`  

The run loop on which the timer runs.

`mode`  

The run loop mode in which to run the timer.

`options`  

Scheduler options passed to the timer. Defaults to `nil`.

## Return Value

A publisher that repeatedly emits the current date on the given interval.

## Discussion

The return type, Timer.TimerPublisher, conforms to ConnectablePublisher, which means you must explicitly connect to the Timer publisher to begin publishing events. You can do this with a call to connect(), or by using autoconnect() to automatically connect when a subscriber attaches, as shown here:

```
cancellable = Timer.publish(every: 1, on: .main, in: .common)
    .autoconnect()
    .sink() {
        print ("timer fired: \($0)")
}

```

## Topics

### Creating a Timer Publisher

init(interval: TimeInterval, tolerance: TimeInterval?, runLoop: RunLoop, mode: RunLoop.Mode, options: RunLoop.SchedulerOptions?)

Creates a publisher that repeatedly emits the current date on the given interval.

## See Also

### Firing Messages as a Combine Publisher

class TimerPublisher

A publisher that repeatedly emits the current date on a given interval.

