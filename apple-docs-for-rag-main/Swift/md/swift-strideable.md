

- Swift
-  Strideable 

Protocol

# Strideable

A type representing continuous, one-dimensional values that can be offset and measured.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Strideable : Comparable
```

## Overview

You can use a type that conforms to the `Strideable` protocol with the `stride(from:to:by:)` and `stride(from:through:by:)` functions. For example, you can use `stride(from:to:by:)` to iterate over an interval of floating-point values:

```
for radians in stride(from: 0.0, to: .pi * 2, by: .pi / 2) {
    let degrees = Int(radians * 180 / .pi)
    print("Degrees: \(degrees), radians: \(radians)")
}
// Degrees: 0, radians: 0.0
// Degrees: 90, radians: 1.5707963267949
// Degrees: 180, radians: 3.14159265358979
// Degrees: 270, radians: 4.71238898038469
```

The last parameter of these functions is of the associated `Stride` type—the type that represents the distance between any two instances of the `Strideable` type.

Types that have an integer `Stride` can be used as the boundaries of a countable range or as the lower bound of an iterable one-sided range. For example, you can iterate over a range of `Int` and use sequence and collection methods.

```
var sum = 0
for x in 1...100 {
    sum += x
}
// sum == 5050

let digits = (0..

# Conforming to the Strideable Protocol

To add `Strideable` conformance to a custom type, choose a `Stride` type that can represent the distance between two instances and implement the `advanced(by:)` and `distance(to:)` methods. For example, this hypothetical `Date` type stores its value as the number of days before or after January 1, 2000:

```
struct Date: Equatable, CustomStringConvertible {
    var daysAfterY2K: Int

    var description: String {
        // ...
    }
}
```

The `Stride` type for `Date` is `Int`, inferred from the parameter and return types of `advanced(by:)` and `distance(to:)`:

```
extension Date: Strideable {
    func advanced(by n: Int) -> Date {
        var result = self
        result.daysAfterY2K += n
        return result
    }

    func distance(to other: Date) -> Int {
        return other.daysAfterY2K - self.daysAfterY2K
    }
}
```

The `Date` type can now be used with the `stride(from:to:by:)` and `stride(from:through:by:)` functions and as the bounds of an iterable range.

```
let startDate = Date(daysAfterY2K: 0)   // January 1, 2000
let endDate = Date(daysAfterY2K: 15)    // January 16, 2000

for date in stride(from: startDate, to: endDate, by: 7) {
    print(date)
}
// January 1, 2000
// January 8, 2000
// January 15, 2000
```

Important

The `Strideable` protocol provides default implementations for the equal-to (`==`) and less-than (`

## Topics

### Getting an Offset Value

func advanced(by: Self.Stride) -> Self

Returns a value that is offset the specified distance from this value.

**Required** Default implementation provided.

static func + (Self, Self.Stride) -> Self

static func + (Self.Stride, Self) -> Self

static func - (Self, Self.Stride) -> Self

static func - (Self, Self) -> Self.Stride

### Comparing Values

func distance(to: Self) -> Self.Stride

Returns the distance from this value to the given value, expressed as a stride.

**Required** Default implementation provided.

### Operators

static func += (inout Self, Self.Stride)

static func -= (inout Self, Self.Stride)

### Associated Types

associatedtype Stride : Comparable, SignedNumeric

A type that represents the distance between two values.

**Required**

## Relationships

### Inherits From

- Comparable
- Equatable

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- FixedWidthInteger
- FloatingPoint
- SignedInteger
- UnsignedInteger

### Conforming Types

- AutoreleasingUnsafeMutablePointer
- Double
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawPointer

## See Also

### Basic Arithmetic

protocol AdditiveArithmetic

A type with values that support addition and subtraction.

protocol Numeric

A type with values that support multiplication.

protocol SignedNumeric

A numeric type with a negation operation.

