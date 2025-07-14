

- Swift
- Task
-  sleep(until:tolerance:clock:) 

Type Method

# sleep(until:tolerance:clock:)

Suspends the current task until the given deadline within a tolerance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func sleep(
    until deadline: C.Instant,
    tolerance: C.Instant.Duration? = nil,
    clock: C = ContinuousClock()
) async throws where C : Clock
```

Available when `Success` is `Never` and `Failure` is `Never`.

## Discussion

If the task is canceled before the time ends, this function throws `CancellationError`.

This function doesn’t block the underlying thread.

```
  try await Task.sleep(until: .now + .seconds(3))
```

## See Also

### Suspending Execution

static func yield() async

Suspends the current task and allows other tasks to execute.

static func sleep(nanoseconds: UInt64) async throws

Suspends the current task for at least the given duration in nanoseconds.

static func sleep&lt;C>(for: C.Instant.Duration, tolerance: C.Instant.Duration?, clock: C) async throws

Suspends the current task for the given duration.

