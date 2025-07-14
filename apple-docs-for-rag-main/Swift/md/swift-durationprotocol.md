

- Swift
-  DurationProtocol 

Protocol

# DurationProtocol

A type that defines a duration for a given `InstantProtocol` type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol DurationProtocol : AdditiveArithmetic, Comparable, Sendable
```

## Topics

### Operators

static func * (Self, Int) -> Self

**Required**

static func *= (inout Self, Int)

**Required** Default implementation provided.

static func / (Self, Self) -> Double

**Required**

static func / (Self, Int) -> Self

**Required**

static func /= (inout Self, Int)

**Required** Default implementation provided.

## Relationships

### Inherits From

- AdditiveArithmetic
- Comparable
- Equatable
- Sendable

### Conforming Types

- Duration

## See Also

### Durations

struct Duration

A representation of high precision time.

