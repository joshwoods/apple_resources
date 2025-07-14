

- Swift
- Result
- Result.Publisher
-  delay(for:tolerance:scheduler:options:) 

Instance Method

# delay(for:tolerance:scheduler:options:)

Delays delivery of all output to the downstream receiver by a specified amount of time on a particular scheduler.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func delay(
    for interval: S.SchedulerTimeType.Stride,
    tolerance: S.SchedulerTimeType.Stride? = nil,
    scheduler: S,
    options: S.SchedulerOptions? = nil
) -> Publishers.Delay where S : Scheduler
```

## Parameters 

`interval`  

The amount of time to delay.

`tolerance`  

The allowed tolerance in delivering delayed events. The `Delay` publisher may deliver elements this much sooner or later than the interval specifies.

`scheduler`  

The scheduler to deliver the delayed events.

`options`  

Options relevant to the scheduler’s behavior.

## Return Value

A publisher that delays delivery of elements and completion to the downstream receiver.

## Discussion

Use delay(for:tolerance:scheduler:options:) when you need to delay the delivery of elements to a downstream by a specified amount of time.

In this example, a Timer publishes an event every second. The delay(for:tolerance:scheduler:options:) operator holds the delivery of the initial element for 3 seconds (±0.5 seconds), after which each element is delivered to the downstream on the main run loop after the specified delay:

```
let df = DateFormatter()
df.dateStyle = .none
df.timeStyle = .long
cancellable = Timer.publish(every: 1.0, on: .main, in: .default)
    .autoconnect()
    .handleEvents(receiveOutput: { date in
        print ("Sending Timestamp \'\(df.string(from: date))\' to delay()")
    })
    .delay(for: .seconds(3), scheduler: RunLoop.main, options: .none)
    .sink(
        receiveCompletion: { print ("completion: \($0)", terminator: "\n") },
        receiveValue: { value in
            let now = Date()
            print ("At \(df.string(from: now)) received  Timestamp \'\(df.string(from: value))\' sent: \(String(format: "%.2f", now.timeIntervalSince(value))) secs ago", terminator: "\n")
        }
    )

// Prints:
//    Sending Timestamp '5:02:33 PM PDT' to delay()
//    Sending Timestamp '5:02:34 PM PDT' to delay()
//    Sending Timestamp '5:02:35 PM PDT' to delay()
//    Sending Timestamp '5:02:36 PM PDT' to delay()
//    At 5:02:36 PM PDT received  Timestamp '5:02:33 PM PDT' sent: 3.00 secs ago
//    Sending Timestamp '5:02:37 PM PDT' to delay()
//    At 5:02:37 PM PDT received  Timestamp '5:02:34 PM PDT' sent: 3.00 secs ago
//    Sending Timestamp '5:02:38 PM PDT' to delay()
//    At 5:02:38 PM PDT received  Timestamp '5:02:35 PM PDT' sent: 3.00 secs ago
```

The delay affects the delivery of elements and completion, but not of the original subscription.

