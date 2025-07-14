

- Swift
-  RawRepresentable 

Protocol

# RawRepresentable

A type that can be converted to and from an associated raw value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol RawRepresentable
```

## Overview

With a `RawRepresentable` type, you can switch back and forth between a custom type and an associated `RawValue` type without losing the value of the original `RawRepresentable` type. Using the raw value of a conforming type streamlines interoperation with Objective-C and legacy APIs and simplifies conformance to other protocols, such as `Equatable`, `Comparable`, and `Hashable`.

The `RawRepresentable` protocol is seen mainly in two categories of types: enumerations with raw value types and option sets.

# Enumerations with Raw Values

For any enumeration with a string, integer, or floating-point raw type, the Swift compiler automatically adds `RawRepresentable` conformance. When defining your own custom enumeration, you give it a raw type by specifying the raw type as the first item in the enumeration’s type inheritance list. You can also use literals to specify values for one or more cases.

For example, the `Counter` enumeration defined here has an `Int` raw value type and gives the first case a raw value of `1`:

```
enum Counter: Int {
    case one = 1, two, three, four, five
}
```

You can create a `Counter` instance from an integer value between 1 and 5 by using the `init?(rawValue:)` initializer declared in the `RawRepresentable` protocol. This initializer is failable because although every case of the `Counter` type has a corresponding `Int` value, there are many `Int` values that *don’t* correspond to a case of `Counter`.

```
for i in 3...6 {
    print(Counter(rawValue: i))
}
// Prints "Optional(Counter.three)"
// Prints "Optional(Counter.four)"
// Prints "Optional(Counter.five)"
// Prints "nil"
```

# Option Sets

Option sets all conform to `RawRepresentable` by inheritance using the `OptionSet` protocol. Whether using an option set or creating your own, you use the raw value of an option set instance to store the instance’s bitfield. The raw value must therefore be of a type that conforms to the `FixedWidthInteger` protocol, such as `UInt8` or `Int`. For example, the `Direction` type defines an option set for the four directions you can move in a game.

```
struct Directions: OptionSet {
    let rawValue: UInt8

    static let up    = Directions(rawValue: 1 

Unlike enumerations, option sets provide a nonfailable `init(rawValue:)` initializer to convert from a raw value, because option sets don’t have an enumerated list of all possible cases. Option set values have a one-to-one correspondence with their associated raw values.

In the case of the `Directions` option set, an instance can contain zero, one, or more of the four defined directions. This example declares a constant with three currently allowed moves. The raw value of the `allowedMoves` instance is the result of the bitwise OR of its three members’ raw values:

```
let allowedMoves: Directions = [.up, .down, .left]
print(allowedMoves.rawValue)
// Prints "7"
```

Option sets use bitwise operations on their associated raw values to implement their mathematical set operations. For example, the `contains()` method on `allowedMoves` performs a bitwise AND operation to check whether the option set contains an element.

```
print(allowedMoves.contains(.right))
// Prints "false"
print(allowedMoves.rawValue & Directions.right.rawValue)
// Prints "0"
```

## Topics

### Creating a Value

init?(rawValue: Self.RawValue)

Creates a new instance with the specified raw value.

**Required**

### Accessing the Raw Value

var rawValue: Self.RawValue

The corresponding value of the raw type.

**Required**

associatedtype RawValue

The raw type that can be used to represent all values of the conforming type.

**Required**

### Comparing Values

func == &lt;T>(T, T) -> Bool

Returns a Boolean value indicating whether the two arguments are equal.

func != &lt;T>(T, T) -> Bool

Returns a Boolean value indicating whether the two arguments are not equal.

func != &lt;T>(T, T) -> Bool

Returns a Boolean value indicating whether the two arguments are not equal.

### Decoding a Value

These initializer overloads are available for any conforming type with a `RawValue` that is a `Decodable` standard library type.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Bool`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Double`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Float`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int8`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int16`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int32`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int64`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt8`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt16`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt32`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt64`.

### Encoding a Value

These overloads are available for any conforming type with a `RawValue` that is an `Encodable` standard library type.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Bool`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Double`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Float`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int8`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int16`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int64`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt8`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt16`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt64`.

### Initializers

init?&lt;T>(codingKey: T)

init?&lt;T>(codingKey: T)

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt128`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int128`.

### Instance Properties

var codingKey: any CodingKey

var codingKey: any CodingKey

var hashValue: Int

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int128`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt128`.

func hash(into: inout Hasher)

### Type Aliases

typealias AtomicOptionalRepresentation

The storage representation type that encodes to and decodes from `Optional` which is a suitable type when used in atomic operations on `Optional`.

typealias AtomicRepresentation

The storage representation type that `Self` encodes to and decodes from which is a suitable type when used in atomic operations.

### Type Methods

static func decodeAtomicOptionalRepresentation(consuming Self.RawValue.AtomicOptionalRepresentation) -> Self?

Recovers the logical atomic type `Self?` by destroying some `AtomicOptionalRepresentation` storage instance returned from an atomic operation on `Optional`.

static func decodeAtomicRepresentation(consuming Self.RawValue.AtomicRepresentation) -> Self

Recovers the logical atomic type `Self` by destroying some `AtomicRepresentation` storage instance returned from an atomic operation.

static func encodeAtomicOptionalRepresentation(consuming Self?) -> Self.RawValue.AtomicOptionalRepresentation

Destroys a value of `Self` and prepares an `AtomicOptionalRepresentation` storage type to be used for atomic operations on `Optional`.

static func encodeAtomicRepresentation(consuming Self) -> Self.RawValue.AtomicRepresentation

Destroys a value of `Self` and prepares an `AtomicRepresentation` storage type to be used for atomic operations.

## Relationships

### Inherited By

- OptionSet

### Conforming Types

- CodingUserInfoKey
- FloatingPointSign
- String.Encoding
- TaskPriority
- Unicode.CanonicalCombiningClass

## See Also

### Raw Representation

protocol CaseIterable

A type that provides a collection of all of its values.

