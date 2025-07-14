

- Combine
- Publishers
- Publishers.Breakpoint
-  throttle(for:scheduler:latest:) 

Instance Method

# throttle(for:scheduler:latest:)

Publishes either the most-recent or first element published by the upstream publisher in the specified time interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func throttle(
    for interval: S.SchedulerTimeType.Stride,
    scheduler: S,
    latest: Bool
) -> Publishers.Throttle where S : Scheduler
```

## Parameters 

`interval`  

The interval at which to find and emit either the most recent or the first element, expressed in the time system of the scheduler.

`scheduler`  

The scheduler on which to publish elements.

`latest`  

A Boolean value that indicates whether to publish the most recent element. If `false`, the publisher emits the first element received during the interval.

## Return Value

A publisher that emits either the most-recent or first element received during the specified interval.

## Discussion

Use throttle(for:scheduler:latest:) to selectively republish elements from an upstream publisher during an interval you specify. Other elements received from the upstream in the throttling interval aren’t republished.

In the example below, a Timer.TimerPublisher produces elements on one-second intervals; the throttle(for:scheduler:latest:) operator delivers the first event, then republishes only the latest event in the following ten second intervals:

```
cancellable = Timer.publish(every: 3.0, on: .main, in: .default)
    .autoconnect()
    .print("\(Date().description)")
    .throttle(for: 10.0, scheduler: RunLoop.main, latest: true)
    .sink(
        receiveCompletion: { print ("Completion: \($0).") },
        receiveValue: { print("Received Timestamp \($0).") }
     )

// Prints:
 //    Publish at: 2020-03-19 18:26:54 +0000: receive value: (2020-03-19 18:26:57 +0000)
 //    Received Timestamp 2020-03-19 18:26:57 +0000.
 //    Publish at: 2020-03-19 18:26:54 +0000: receive value: (2020-03-19 18:27:00 +0000)
 //    Publish at: 2020-03-19 18:26:54 +0000: receive value: (2020-03-19 18:27:03 +0000)
 //    Publish at: 2020-03-19 18:26:54 +0000: receive value: (2020-03-19 18:27:06 +0000)
 //    Publish at: 2020-03-19 18:26:54 +0000: receive value: (2020-03-19 18:27:09 +0000)
 //    Received Timestamp 2020-03-19 18:27:09 +0000.
```

## See Also

### Controlling Timing

func measureInterval&lt;S>(using: S, options: S.SchedulerOptions?) -> Publishers.MeasureInterval&lt;Self, S>

Measures and emits the time interval between events received from an upstream publisher.

func debounce&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Debounce&lt;Self, S>

Publishes elements only after a specified time interval elapses between events.

func delay&lt;S>(for: S.SchedulerTimeType.Stride, tolerance: S.SchedulerTimeType.Stride?, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Delay&lt;Self, S>

Delays delivery of all output to the downstream receiver by a specified amount of time on a particular scheduler.

func timeout&lt;S>(S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?, customError: (() -> Self.Failure)?) -> Publishers.Timeout&lt;Self, S>

Terminates publishing if the upstream publisher exceeds the specified time interval without producing an element.

