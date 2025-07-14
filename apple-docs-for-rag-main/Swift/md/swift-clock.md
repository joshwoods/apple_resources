

- Swift
-  Clock 

Protocol

# Clock

A mechanism in which to measure time, and delay work until a given point in time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol Clock : Sendable
```

## Overview

Types that conform to the `Clock` protocol define a concept of “now” which is the specific instant in time that property is accessed. Any pair of calls to the `now` property may have a minimum duration between them - this minimum resolution is exposed by the `minimumResolution` property to inform any user of the type the expected granularity of accuracy.

One of the primary uses for clocks is to schedule task sleeping. This method resumes the calling task after a given deadline has been met or passed with a given tolerance value. The tolerance is expected as a leeway around the deadline. The clock may reschedule tasks within the tolerance to ensure efficient execution of resumptions by reducing potential operating system wake-ups. If no tolerance is specified (i.e. nil is passed in) the sleep function is expected to schedule with a default tolerance strategy.

For more information about specific clocks see `ContinuousClock` and `SuspendingClock`.

## Topics

### Associated Types

associatedtype Duration

**Required**

associatedtype Instant : InstantProtocol

**Required**

### Instance Properties

var minimumResolution: Self.Duration

**Required**

var now: Self.Instant

**Required**

### Instance Methods

func measure(() throws -> Void) rethrows -> Self.Instant.Duration

Measure the elapsed time to execute a closure.

func measure(isolation: isolated (any Actor)?, () async throws -> Void) async rethrows -> Self.Instant.Duration

Measure the elapsed time to execute an asynchronous closure.

func sleep(for: Self.Instant.Duration, tolerance: Self.Instant.Duration?) async throws

Suspends for the given duration.

func sleep(until: Self.Instant, tolerance: Self.Instant.Duration?) async throws

**Required**

### Type Properties

static var continuous: ContinuousClock

A clock that measures time that always increments but does not stop incrementing while the system is asleep.

static var suspending: SuspendingClock

A clock that measures time that always increments but stops incrementing while the system is asleep.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- ContinuousClock
- SuspendingClock

## See Also

### Clocks

struct ContinuousClock

A clock that measures time that always increments and does not stop incrementing while the system is asleep.

struct SuspendingClock

A clock that measures time that always increments but stops incrementing while the system is asleep.

