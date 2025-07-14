

- Swift
- Task
-  sleep(nanoseconds:) 

Type Method

# sleep(nanoseconds:)

Suspends the current task for at least the given duration in nanoseconds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func sleep(nanoseconds duration: UInt64) async throws
```

Available when `Success` is `Never` and `Failure` is `Never`.

## Discussion

If the task is canceled before the time ends, this function throws `CancellationError`.

This function doesn’t block the underlying thread.

## See Also

### Suspending Execution

static func yield() async

Suspends the current task and allows other tasks to execute.

static func sleep&lt;C>(for: C.Instant.Duration, tolerance: C.Instant.Duration?, clock: C) async throws

Suspends the current task for the given duration.

static func sleep&lt;C>(until: C.Instant, tolerance: C.Instant.Duration?, clock: C) async throws

Suspends the current task until the given deadline within a tolerance.

