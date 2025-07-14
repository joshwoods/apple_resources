

- Swift
-  PartialRangeThrough 

Structure

# PartialRangeThrough

A partial interval up to, and including, an upper bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct PartialRangeThrough where Bound : Comparable
```

## Overview

You create `PartialRangeThrough` instances by using the prefix closed range operator (prefix `...`).

```
let throughFive = ...5.0
```

You can use a `PartialRangeThrough` instance to quickly check if a value is contained in a particular range of values. For example:

```
throughFive.contains(4.0)     // true
throughFive.contains(5.0)     // true
throughFive.contains(6.0)     // false
```

You can use a `PartialRangeThrough` instance of a collection’s indices to represent the range from the start of the collection up to, and including, the partial range’s upper bound.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[...3])
// Prints "[10, 20, 30, 40]"
```

## Topics

### Initializers

init(Bound)

### Instance Properties

let upperBound: Bound

### Default Implementations

CustomTestStringConvertible Implementations

Decodable Implementations

Encodable Implementations

RangeExpression Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Bound` conforms to `Comparable`.

- CustomTestStringConvertible
- Decodable

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- Encodable

  Conforms when `Bound` conforms to `Comparable` and `Encodable`.

- MLShapedArrayRangeExpression
- MLTensorRangeExpression
- RangeExpression

  Conforms when `Bound` conforms to `Comparable`.

- Sendable

  Conforms when `Bound` conforms to `Comparable` and `Sendable`.

## See Also

### Range Expressions

struct PartialRangeUpTo

A partial half-open interval up to, but not including, an upper bound.

struct PartialRangeFrom

A partial interval extending upward from a lower bound.

protocol RangeExpression

A type that can be used to slice a collection.

enum UnboundedRange_

A range expression that represents the entire range of a collection.

