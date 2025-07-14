

- Swift
-  CustomStringConvertible 

Protocol

# CustomStringConvertible

A type with a customized textual representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol CustomStringConvertible
```

## Overview

Types that conform to the `CustomStringConvertible` protocol can provide their own representation to be used when converting an instance to a string. The `String(describing:)` initializer is the preferred way to convert an instance of *any* type to a string. If the passed instance conforms to `CustomStringConvertible`, the `String(describing:)` initializer and the `print(_:)` function use the instance’s custom `description` property.

Accessing a type’s `description` property directly or using `CustomStringConvertible` as a generic constraint is discouraged.

# Conforming to the CustomStringConvertible Protocol

Add `CustomStringConvertible` conformance to your custom types by defining a `description` property.

For example, this custom `Point` struct uses the default representation supplied by the standard library:

```
struct Point {
    let x: Int, y: Int
}

let p = Point(x: 21, y: 30)
print(p)
// Prints "Point(x: 21, y: 30)"
```

After implementing the `description` property and declaring `CustomStringConvertible` conformance, the `Point` type provides its own custom representation.

```
extension Point: CustomStringConvertible {
    var description: String {
        return "(\(x), \(y))"
    }
}

print(p)
// Prints "(21, 30)"
```

## Topics

### Instance Properties

var description: String

A textual representation of this instance.

**Required** Default implementations provided.

## Relationships

### Inherited By

- BinaryInteger
- CodingKey
- FixedWidthInteger
- LosslessStringConvertible
- SIMD
- SignedInteger
- StringProtocol
- UnsignedInteger

### Conforming Types

- AnyHashable
- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AtomicLoadOrdering
- AtomicStoreOrdering
- AtomicUpdateOrdering
- Bool
- Character
- ClosedRange

  Conforms when `Bound` conforms to `Comparable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DefaultStringInterpolation
- Dictionary

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Keys

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Values

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- DiscontiguousSlice

  Conforms when `Base` conforms to `Collection`.

- DiscontiguousSlice.Index

  Conforms when `Base` conforms to `Collection`.

- Double
- Duration
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- KeyValuePairs

  Conforms when `Key` conforms to `Copyable`, `Key` conforms to `Escapable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Mirror
- Range

  Conforms when `Bound` conforms to `Comparable`.

- RangeSet

  Conforms when `Bound` conforms to `Comparable`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable`.

- RemoteCallTarget
- SIMD16
- SIMD2
- SIMD3
- SIMD32
- SIMD4
- SIMD64
- SIMD8
- SIMDMask
- Set

  Conforms when `Element` conforms to `Hashable`.

- StaticString
- String
- String.Encoding
- String.UTF16View
- String.UTF8View
- String.UnicodeScalarView
- Substring
- TaskLocal
- TaskPriority
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- Unicode.Scalar
- UnownedJob
- WordPair

## See Also

### String Representation

protocol LosslessStringConvertible

A type that can be represented as a string in a lossless, unambiguous way.

protocol CustomDebugStringConvertible

A type with a customized textual representation suitable for debugging purposes.

