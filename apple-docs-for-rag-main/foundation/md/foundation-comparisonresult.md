

- Foundation
-  ComparisonResult 

Enumeration

# ComparisonResult

Constants that indicate sort order.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum ComparisonResult
```

## Overview

These constants are used to indicate how items in a request are ordered, from the first one given in a method invocation or function call to the last (that is, left to right in code).

## Topics

### Constants

case orderedAscending

The left operand is smaller than the right operand.

case orderedSame

The two operands are equal.

case orderedDescending

The left operand is greater than the right operand.

case orderedAscending

The left operand is smaller than the right operand.

case orderedSame

The two operands are equal.

case orderedDescending

The left operand is greater than the right operand.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sorting

class NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

struct SortDescriptor

A serializable description of how to sort numerics and strings.

protocol SortComparator

A comparison algorithm for a specified type.

struct ComparableComparator

A comparator that compares types according to their conformance to the comparable protocol.

struct KeyPathComparator

A comparator that uses another sort comparator to provide the comparison of values at a key path.

enum SortOrder

The orderings that you can perform sorts with.

