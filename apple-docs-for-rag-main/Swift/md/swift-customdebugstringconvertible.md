

- Swift
-  CustomDebugStringConvertible 

Protocol

# CustomDebugStringConvertible

A type with a customized textual representation suitable for debugging purposes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol CustomDebugStringConvertible
```

## Overview

Swift provides a default debugging textual representation for any type. That default representation is used by the `String(reflecting:)` initializer and the `debugPrint(_:)` function for types that don’t provide their own. To customize that representation, make your type conform to the `CustomDebugStringConvertible` protocol.

Because the `String(reflecting:)` initializer works for instances of *any* type, returning an instance’s `debugDescription` if the value passed conforms to `CustomDebugStringConvertible`, accessing a type’s `debugDescription` property directly or using `CustomDebugStringConvertible` as a generic constraint is discouraged.

Note

Calling the `dump(_:_:_:_:)` function and printing in the debugger uses both `String(reflecting:)` and `Mirror(reflecting:)` to collect information about an instance. If you implement `CustomDebugStringConvertible` conformance for your custom type, you may want to consider providing a custom mirror by implementing `CustomReflectable` conformance, as well.

# Conforming to the CustomDebugStringConvertible Protocol

Add `CustomDebugStringConvertible` conformance to your custom types by defining a `debugDescription` property.

For example, this custom `Point` struct uses the default representation supplied by the standard library:

```
struct Point {
    let x: Int, y: Int
}

let p = Point(x: 21, y: 30)
print(String(reflecting: p))
// Prints "Point(x: 21, y: 30)"
```

After adding `CustomDebugStringConvertible` conformance by implementing the `debugDescription` property, `Point` provides its own custom debugging representation.

```
extension Point: CustomDebugStringConvertible {
    var debugDescription: String {
        return "(\(x), \(y))"
    }
}

print(String(reflecting: p))
// Prints "(21, 30)"
```

## Topics

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

**Required** Default implementation provided.

## Relationships

### Inherited By

- CodingKey

### Conforming Types

- AnyHashable
- AnyKeyPath
- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AutoreleasingUnsafeMutablePointer
- CVaListPointer
- Character
- ClosedRange

  Conforms when `Bound` conforms to `Comparable`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Dictionary

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Keys

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Values

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Double
- Float
- Float16
- Float80
- KeyPath
- KeyValuePairs

  Conforms when `Key` conforms to `Copyable`, `Key` conforms to `Escapable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- ObjectIdentifier
- OpaquePointer
- Optional

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- PartialKeyPath
- Range

  Conforms when `Bound` conforms to `Comparable`.

- ReferenceWritableKeyPath
- SIMD16

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD2

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD3

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD32

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD4

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD64

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD8

  Conforms when `Scalar` conforms to `SIMDScalar`.

- Set

  Conforms when `Element` conforms to `Hashable`.

- StaticBigInt
- StaticString
- String
- String.Index
- String.UTF16View
- String.UTF8View
- String.UnicodeScalarView
- Substring
- Unicode.Scalar
- UnsafeBufferPointer

  Conforms when `Element` conforms to `Escapable`.

- UnsafeMutableBufferPointer

  Conforms when `Element` conforms to `Escapable`.

- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawBufferPointer
- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawBufferPointer
- UnsafeRawPointer
- WordPair
- WritableKeyPath

## See Also

### String Representation

protocol CustomStringConvertible

A type with a customized textual representation.

protocol LosslessStringConvertible

A type that can be represented as a string in a lossless, unambiguous way.

