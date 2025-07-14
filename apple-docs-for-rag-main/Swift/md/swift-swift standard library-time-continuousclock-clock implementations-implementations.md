

- Swift
- Swift Standard Library
- Time
- ContinuousClock
-  Clock Implementations 

API Collection

# Clock Implementations

## Topics

### Instance Properties

var minimumResolution: Duration

The minimum non-zero resolution between any two calls to `now`.

var now: ContinuousClock.Instant

The current continuous instant.

### Instance Methods

func measure(() throws -> Void) rethrows -> Self.Instant.Duration

Measure the elapsed time to execute a closure.

func measure(isolation: isolated (any Actor)?, () async throws -> Void) async rethrows -> Self.Instant.Duration

Measure the elapsed time to execute an asynchronous closure.

func sleep(for: Self.Instant.Duration, tolerance: Self.Instant.Duration?) async throws

Suspends for the given duration.

func sleep(until: ContinuousClock.Instant, tolerance: Duration?) async throws

Suspend task execution until a given deadline within a tolerance. If no tolerance is specified then the system may adjust the deadline to coalesce CPU wake-ups to more efficiently process the wake-ups in a more power efficient manner.

### Type Aliases

typealias Duration

### Type Properties

static var continuous: ContinuousClock

A clock that measures time that always increments but does not stop incrementing while the system is asleep.

