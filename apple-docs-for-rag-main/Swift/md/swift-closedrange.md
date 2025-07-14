

- Swift
-  ClosedRange 

Structure

# ClosedRange

An interval from a lower bound up to, and including, an upper bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ClosedRange where Bound : Comparable
```

## Overview

You create a `ClosedRange` instance by using the closed range operator (`...`).

```
let throughFive = 0...5
```

A `ClosedRange` instance contains both its lower bound and its upper bound.

```
throughFive.contains(3)
// true
throughFive.contains(10)
// false
throughFive.contains(5)
// true
```

Because a closed range includes its upper bound, a closed range whose lower bound is equal to the upper bound contains that value. Therefore, a `ClosedRange` instance cannot represent an empty range.

```
let zeroInclusive = 0...0
zeroInclusive.contains(0)
// true
zeroInclusive.isEmpty
// false
```

## Using a Closed Range as a Collection of Consecutive Values

When a closed range uses integers as its lower and upper bounds, or any other type that conforms to the `Strideable` protocol with an integer stride, you can use that range in a `for`-`in` loop or with any sequence or collection method. The elements of the range are the consecutive values from its lower bound up to, and including, its upper bound.

```
for n in 3...5 {
    print(n)
}
// Prints "3"
// Prints "4"
// Prints "5"
```

Because floating-point types such as `Float` and `Double` are their own `Stride` types, they cannot be used as the bounds of a countable range. If you need to iterate over consecutive floating-point values, see the `stride(from:through:by:)` function.

## Topics

### Creating a Range

Create a new range using the closed range operator (`...`).

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

### Converting Ranges

func relative&lt;C>(to: C) -> Range&lt;Bound>

Returns the range of indices described by this range expression within the given collection.

### Inspecting a Range

var isEmpty: Bool

A Boolean value indicating whether the range contains no elements.

let lowerBound: Bound

The range’s lower bound.

let upperBound: Bound

The range’s upper bound.

### Checking for Containment

static func ~= (Self, Self.Bound) -> Bool

Returns a Boolean value indicating whether a value is included in a range.

### Clamping a Range

func clamped(to: ClosedRange&lt;Bound>) -> ClosedRange&lt;Bound>

Returns a copy of this range clamped to the given limiting range.

### Comparing Ranges

static func == (ClosedRange&lt;Bound>, ClosedRange&lt;Bound>) -> Bool

Returns a Boolean value indicating whether two ranges are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func overlaps(Range&lt;Bound>) -> Bool

Returns a Boolean value indicating whether this range and the given range contain an element in common.

func overlaps(ClosedRange&lt;Bound>) -> Bool

Returns a Boolean value indicating whether this range and the given closed range contain an element in common.

### Manipulating Indices

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Describing a Range

var description: String

A textual representation of the range.

var debugDescription: String

A textual representation of the range, suitable for debugging.

var customMirror: Mirror

The custom mirror for this instance.

### Encoding and Decoding a Range

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Infrequently Used Functionality

init(uncheckedBounds: (lower: Bound, upper: Bound))

Creates an instance with the given bounds.

var hashValue: Int

The hash value.

### Initializers

init(Range&lt;Bound>)

Creates an instance equivalent to the given `Range`.

init(ClosedRange&lt;Bound>)

Now that Range is conditionally a collection when Bound: Strideable, CountableRange is no longer needed. This is a deprecated initializer for any remaining uses of Range(countableRange).

### Instance Methods

func contains(Range&lt;Bound>) -> Bool

Returns a Boolean value indicating whether the given range is contained within this closed range.

func contains(ClosedRange&lt;Bound>) -> Bool

Returns a Boolean value indicating whether the given closed range is contained within this closed range.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

CustomTestStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

RangeExpression Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- Collection

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- Copyable

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- CustomDebugStringConvertible

  Conforms when `Bound` conforms to `Comparable`.

- CustomReflectable

  Conforms when `Bound` conforms to `Comparable`.

- CustomStringConvertible

  Conforms when `Bound` conforms to `Comparable`.

- CustomTestStringConvertible
- Decodable

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- Encodable

  Conforms when `Bound` conforms to `Comparable` and `Encodable`.

- Equatable

  Conforms when `Bound` conforms to `Comparable`.

- Hashable

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- MLShapedArrayRangeExpression
- MLTensorRangeExpression
- PositionScaleRange
- RandomAccessCollection

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- RangeExpression

  Conforms when `Bound` conforms to `Comparable`.

- ScaleDomain
- ScaleRange
- Sendable

  Conforms when `Bound` conforms to `Comparable` and `Sendable`.

- Sequence

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## See Also

### Ranges

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

struct Range

A half-open interval from a lower bound up to, but not including, an upper bound.

struct RangeSet

A set of values of any comparable type, represented by ranges.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

