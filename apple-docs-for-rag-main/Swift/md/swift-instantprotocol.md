

- Swift
-  InstantProtocol 

Protocol

# InstantProtocol

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol InstantProtocol : Comparable, Hashable, Sendable
```

## Topics

### Associated Types

associatedtype Duration : DurationProtocol

**Required**

### Instance Methods

func advanced(by: Self.Duration) -> Self

**Required**

func duration(to: Self) -> Self.Duration

**Required**

## Relationships

### Inherits From

- Comparable
- Equatable
- Hashable
- Sendable

### Conforming Types

- ContinuousClock.Instant
- SuspendingClock.Instant

