

- Swift
-  RangeExpression 

Protocol

# RangeExpression

A type that can be used to slice a collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol RangeExpression
```

## Overview

A type that conforms to `RangeExpression` can convert itself to a `Range` of indices within a given collection.

## Topics

### Operators

static func ~= (Self, Self.Bound) -> Bool

Returns a Boolean value indicating whether a value is included in a range.

### Associated Types

associatedtype Bound : Comparable

The type for which the expression describes a range.

**Required**

### Instance Methods

func contains(Self.Bound) -> Bool

Returns a Boolean value indicating whether the given element is contained within the range expression.

**Required**

func relative&lt;C>(to: C) -> Range&lt;Self.Bound>

Returns the range of indices described by this range expression within the given collection.

**Required**

## Relationships

### Conforming Types

- ClosedRange

  Conforms when `Bound` conforms to `Comparable`.

- PartialRangeFrom

  Conforms when `Bound` conforms to `Comparable`.

- PartialRangeThrough

  Conforms when `Bound` conforms to `Comparable`.

- PartialRangeUpTo

  Conforms when `Bound` conforms to `Comparable`.

- Range

  Conforms when `Bound` conforms to `Comparable`.

## See Also

### Range Expressions

struct PartialRangeUpTo

A partial half-open interval up to, but not including, an upper bound.

struct PartialRangeThrough

A partial interval up to, and including, an upper bound.

struct PartialRangeFrom

A partial interval extending upward from a lower bound.

enum UnboundedRange_

A range expression that represents the entire range of a collection.

