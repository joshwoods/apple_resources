

- Swift
-  PartialRangeFrom 

Structure

# PartialRangeFrom

A partial interval extending upward from a lower bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct PartialRangeFrom where Bound : Comparable
```

## Overview

You create `PartialRangeFrom` instances by using the postfix range operator (postfix `...`).

```
let atLeastFive = 5...
```

You can use a partial range to quickly check if a value is contained in a particular range of values. For example:

```
atLeastFive.contains(4)
// false
atLeastFive.contains(5)
// true
atLeastFive.contains(6)
// true
```

You can use a partial range of a collection’s indices to represent the range from the partial range’s lower bound up to the end of the collection.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[3...])
// Prints "[40, 50, 60, 70]"
```

## Using a Partial Range as a Sequence

When a partial range uses integers as its lower and upper bounds, or any other type that conforms to the `Strideable` protocol with an integer stride, you can use that range in a `for`-`in` loop or with any sequence method that doesn’t require that the sequence is finite. The elements of a partial range are the consecutive values from its lower bound continuing upward indefinitely.

```
func isTheMagicNumber(_ x: Int) -> Bool {
    return x == 3
}

for x in 1... {
    if isTheMagicNumber(x) {
        print("\(x) is the magic number!")
        break
    } else {
        print("\(x) wasn't it...")
    }
}
// "1 wasn't it..."
// "2 wasn't it..."
// "3 is the magic number!"
```

Because a `PartialRangeFrom` sequence counts upward indefinitely, do not use one with methods that read the entire sequence before returning, such as `map(_:)`, `filter(_:)`, or `suffix(_:)`. It is safe to use operations that put an upper limit on the number of elements they access, such as `prefix(_:)` or `dropFirst(_:)`, and operations that you can guarantee will terminate, such as passing a closure you know will eventually return `true` to `first(where:)`.

In the following example, the `asciiTable` sequence is made by zipping together the characters in the `alphabet` string with a partial range starting at 65, the ASCII value of the capital letter A. Iterating over two zipped sequences continues only as long as the shorter of the two sequences, so the iteration stops at the end of `alphabet`.

```
let alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
let asciiTable = zip(65..., alphabet)
for (code, letter) in asciiTable {
    print(code, letter)
}
// "65 A"
// "66 B"
// "67 C"
// ...
// "89 Y"
// "90 Z"
```

The behavior of incrementing indefinitely is determined by the type of `Bound`. For example, iterating over an instance of `PartialRangeFrom` traps when the sequence’s next value would be above `Int.max`.

## Topics

### Initializers

init(Bound)

### Instance Properties

let lowerBound: Bound

### Default Implementations

CustomTestStringConvertible Implementations

Decodable Implementations

Encodable Implementations

RangeExpression Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Bound` conforms to `Comparable` and `Encodable`.

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

- Sequence

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## See Also

### Range Expressions

struct PartialRangeUpTo

A partial half-open interval up to, but not including, an upper bound.

struct PartialRangeThrough

A partial interval up to, and including, an upper bound.

protocol RangeExpression

A type that can be used to slice a collection.

enum UnboundedRange_

A range expression that represents the entire range of a collection.

