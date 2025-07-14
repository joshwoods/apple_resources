

- Combine
- Publishers
- Publishers.Sequence
-  timeout(\_:scheduler:options:customError:) 

Instance Method

# timeout(\_:scheduler:options:customError:)

Terminates publishing if the upstream publisher exceeds the specified time interval without producing an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func timeout(
    _ interval: S.SchedulerTimeType.Stride,
    scheduler: S,
    options: S.SchedulerOptions? = nil,
    customError: (() -> Self.Failure)? = nil
) -> Publishers.Timeout where S : Scheduler
```

## Parameters 

`interval`  

The maximum time interval the publisher can go without emitting an element, expressed in the time system of the scheduler.

`scheduler`  

The scheduler on which to deliver events.

`options`  

Scheduler options that customize the delivery of elements.

`customError`  

A closure that executes if the publisher times out. The publisher sends the failure returned by this closure to the subscriber as the reason for termination.

## Return Value

A publisher that terminates if the specified interval elapses with no events received from the upstream publisher.

## Discussion

Use timeout(_:scheduler:options:customError:) to terminate a publisher if an element isn’t delivered within a timeout interval you specify.

In the example below, a PassthroughSubject publishes String elements and is configured to time out if no new elements are received within its `TIME_OUT` window of 5 seconds. A single value is published after the specified 2-second `WAIT_TIME`, after which no more elements are available; the publisher then times out and completes normally.

```
var WAIT_TIME : Int = 2
var TIMEOUT_TIME : Int = 5

let subject = PassthroughSubject()
let cancellable = subject
    .timeout(.seconds(TIMEOUT_TIME), scheduler: DispatchQueue.main, options: nil, customError:nil)
    .sink(
          receiveCompletion: { print ("completion: \($0) at \(Date())") },
          receiveValue: { print ("value: \($0) at \(Date())") }
     )

DispatchQueue.main.asyncAfter(deadline: .now() + .seconds(WAIT_TIME),
                              execute: { subject.send("Some data - sent after a delay of \(WAIT_TIME) seconds") } )

// Prints: value: Some data - sent after a delay of 2 seconds at 2020-03-10 23:47:59 +0000
//         completion: finished at 2020-03-10 23:48:04 +0000
```

If `customError` is `nil`, the publisher completes normally; if you provide a closure for the `customError` argument, the upstream publisher is instead terminated upon timeout, and the error is delivered to the downstream.

## See Also

### Controlling Timing

func measureInterval&lt;S>(using: S, options: S.SchedulerOptions?) -> Publishers.MeasureInterval&lt;Self, S>

Measures and emits the time interval between events received from an upstream publisher.

func debounce&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Debounce&lt;Self, S>

Publishes elements only after a specified time interval elapses between events.

func delay&lt;S>(for: S.SchedulerTimeType.Stride, tolerance: S.SchedulerTimeType.Stride?, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Delay&lt;Self, S>

Delays delivery of all output to the downstream receiver by a specified amount of time on a particular scheduler.

func throttle&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, latest: Bool) -> Publishers.Throttle&lt;Self, S>

Publishes either the most-recent or first element published by the upstream publisher in the specified time interval.

