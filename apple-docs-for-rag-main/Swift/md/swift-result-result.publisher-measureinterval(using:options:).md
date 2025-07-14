

- Swift
- Result
- Result.Publisher
-  measureInterval(using:options:) 

Instance Method

# measureInterval(using:options:)

Measures and emits the time interval between events received from an upstream publisher.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func measureInterval(
    using scheduler: S,
    options: S.SchedulerOptions? = nil
) -> Publishers.MeasureInterval where S : Scheduler
```

## Parameters 

`scheduler`  

A scheduler to use for tracking the timing of events.

`options`  

Options that customize the delivery of elements.

## Return Value

A publisher that emits elements representing the time interval between the elements it receives.

## Discussion

Use measureInterval(using:options:) to measure the time between events delivered from an upstream publisher.

In the example below, a 1-second Timer is used as the data source for an event publisher; the measureInterval(using:options:) operator reports the elapsed time between the reception of events on the main run loop:

```
cancellable = Timer.publish(every: 1, on: .main, in: .default)
    .autoconnect()
    .measureInterval(using: RunLoop.main)
    .sink { print("\($0)", terminator: "\n") }

// Prints:
//      Stride(magnitude: 1.0013610124588013)
//      Stride(magnitude: 0.9992760419845581)
```

The output type of the returned publisher is the time interval of the provided scheduler.

This operator uses the provided scheduler’s `Scheduler/now` property to measure intervals between events.

