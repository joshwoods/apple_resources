

- Foundation
- Timer
-  Timer.TimerPublisher 

Class

# Timer.TimerPublisher

A publisher that repeatedly emits the current date on a given interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class TimerPublisher
```

## Topics

### Initializers

init(interval: TimeInterval, tolerance: TimeInterval?, runLoop: RunLoop, mode: RunLoop.Mode, options: RunLoop.SchedulerOptions?)

Creates a publisher that repeatedly emits the current date on the given interval.

### Instance Properties

let interval: TimeInterval

let mode: RunLoop.Mode

let options: RunLoop.SchedulerOptions?

let runLoop: RunLoop

let tolerance: TimeInterval?

## Relationships

### Conforms To

- ConnectablePublisher
- Publisher

## See Also

### Firing Messages as a Combine Publisher

static func publish(every: TimeInterval, tolerance: TimeInterval?, on: RunLoop, in: RunLoop.Mode, options: RunLoop.SchedulerOptions?) -> Timer.TimerPublisher

Returns a publisher that repeatedly emits the current date on the given interval.

