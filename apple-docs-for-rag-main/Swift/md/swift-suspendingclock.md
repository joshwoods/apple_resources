

- Swift
-  SuspendingClock 

Structure

# SuspendingClock

A clock that measures time that always increments but stops incrementing while the system is asleep.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct SuspendingClock
```

## Overview

`SuspendingClock` can be considered as a system awake time clock. The frame of reference of the `Instant` may be bound machine boot or some other locally defined reference point. This means that the instants are only comparable on the same machine in the same booted session.

This clock is suitable for high resolution measurements of execution.

## Topics

### Structures

struct Instant

### Initializers

init()

### Type Properties

static var now: SuspendingClock.Instant

The current instant accounting for machine suspension.

### Default Implementations

Clock Implementations

## Relationships

### Conforms To

- Clock
- Copyable
- Sendable

## See Also

### Clocks

protocol Clock

A mechanism in which to measure time, and delay work until a given point in time.

struct ContinuousClock

A clock that measures time that always increments and does not stop incrementing while the system is asleep.

