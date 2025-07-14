

- Swift
-  Equatable 

Protocol

# Equatable

A type that can be compared for value equality.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Equatable
```

## Mentioned in 

Adopting Common Protocols

## Overview

Types that conform to the `Equatable` protocol can be compared for equality using the equal-to operator (`==`) or inequality using the not-equal-to operator (`!=`). Most basic types in the Swift standard library conform to `Equatable`.

Some sequence and collection operations can be used more simply when the elements conform to `Equatable`. For example, to check whether an array contains a particular value, you can pass the value itself to the `contains(_:)` method when the array’s element conforms to `Equatable` instead of providing a closure that determines equivalence. The following example shows how the `contains(_:)` method can be used with an array of strings.

```
let students = ["Kofi", "Abena", "Efua", "Kweku", "Akosua"]

let nameToCheck = "Kofi"
if students.contains(nameToCheck) {
    print("\(nameToCheck) is signed up!")
} else {
    print("No record of \(nameToCheck).")
}
// Prints "Kofi is signed up!"
```

# Conforming to the Equatable Protocol

Adding `Equatable` conformance to your custom types means that you can use more convenient APIs when searching for particular instances in a collection. `Equatable` is also the base protocol for the `Hashable` and `Comparable` protocols, which allow more uses of your custom type, such as constructing sets or sorting the elements of a collection.

You can rely on automatic synthesis of the `Equatable` protocol’s requirements for a custom type when you declare `Equatable` conformance in the type’s original declaration and your type meets these criteria:

- For a `struct`, all its stored properties must conform to `Equatable`.

- For an `enum`, all its associated values must conform to `Equatable`. (An `enum` without associated values has `Equatable` conformance even without the declaration.)

To customize your type’s `Equatable` conformance, to adopt `Equatable` in a type that doesn’t meet the criteria listed above, or to extend an existing type to conform to `Equatable`, implement the equal-to operator (`==`) as a static method of your type. The standard library provides an implementation for the not-equal-to operator (`!=`) for any `Equatable` type, which calls the custom `==` function and negates its result.

As an example, consider a `StreetAddress` class that holds the parts of a street address: a house or building number, the street name, and an optional unit number. Here’s the initial declaration of the `StreetAddress` type:

```
class StreetAddress {
    let number: String
    let street: String
    let unit: String?

    init(_ number: String, _ street: String, unit: String? = nil) {
        self.number = number
        self.street = street
        self.unit = unit
    }
}
```

Now suppose you have an array of addresses that you need to check for a particular address. To use the `contains(_:)` method without including a closure in each call, extend the `StreetAddress` type to conform to `Equatable`.

```
extension StreetAddress: Equatable {
    static func == (lhs: StreetAddress, rhs: StreetAddress) -> Bool {
        return
            lhs.number == rhs.number &&
            lhs.street == rhs.street &&
            lhs.unit == rhs.unit
    }
}
```

The `StreetAddress` type now conforms to `Equatable`. You can use `==` to check for equality between any two instances or call the `Equatable`-constrained `contains(_:)` method.

```
let addresses = [StreetAddress("1490", "Grove Street"),
                 StreetAddress("2119", "Maple Avenue"),
                 StreetAddress("1400", "16th Street")]
let home = StreetAddress("1400", "16th Street")

print(addresses[0] == home)
// Prints "false"
print(addresses.contains(home))
// Prints "true"
```

Equality implies substitutability—any two instances that compare equally can be used interchangeably in any code that depends on their values. To maintain substitutability, the `==` operator should take into account all visible aspects of an `Equatable` type. Exposing nonvalue aspects of `Equatable` types other than class identity is discouraged, and any that *are* exposed should be explicitly pointed out in documentation.

Since equality between instances of `Equatable` types is an equivalence relation, any of your custom types that conform to `Equatable` must satisfy three conditions, for any values `a`, `b`, and `c`:

- `a == a` is always `true` (Reflexivity)

- `a == b` implies `b == a` (Symmetry)

- `a == b` and `b == c` implies `a == c` (Transitivity)

Moreover, inequality is the inverse of equality, so any custom implementation of the `!=` operator must guarantee that `a != b` implies `!(a == b)`. The default implementation of the `!=` operator function satisfies this requirement.

## Equality is Separate From Identity

The identity of a class instance is not part of an instance’s value. Consider a class called `IntegerRef` that wraps an integer value. Here’s the definition for `IntegerRef` and the `==` function that makes it conform to `Equatable`:

```
class IntegerRef: Equatable {
    let value: Int
    init(_ value: Int) {
        self.value = value
    }

    static func == (lhs: IntegerRef, rhs: IntegerRef) -> Bool {
        return lhs.value == rhs.value
    }
}
```

The implementation of the `==` function returns the same value whether its two arguments are the same instance or are two different instances with the same integer stored in their `value` properties. For example:

```
let a = IntegerRef(100)
let b = IntegerRef(100)

print(a == a, a == b, separator: ", ")
// Prints "true, true"
```

Class instance identity, on the other hand, is compared using the triple-equals identical-to operator (`===`). For example:

```
let c = a
print(c === a, c === b, separator: ", ")
// Prints "true, false"
```

## Topics

### Equatable Requirements

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

**Required** Default implementations provided.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Tuple Comparison

Compare tuples of between two and six `Equatable` elements for equality or inequality.

func == ((), ()) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func != ((), ()) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

### Pattern Matching

func ~= &lt;T>(T, T) -> Bool

Returns a Boolean value indicating whether two arguments match by value equality.

## Relationships

### Inherited By

- AdditiveArithmetic
- BinaryFloatingPoint
- BinaryInteger
- Comparable
- DistributedActor
- DurationProtocol
- FixedWidthInteger
- FloatingPoint
- Hashable
- InstantProtocol
- Numeric
- OptionSet
- SIMD
- SetAlgebra
- SignedInteger
- SignedNumeric
- Strideable
- StringProtocol
- UnsignedInteger

### Conforming Types

- AnyHashable
- AnyIndex
- AnyKeyPath
- Array

  Conforms when `Element` conforms to `Equatable`.

- ArraySlice

  Conforms when `Element` conforms to `Hashable`.

- AsyncStream.Continuation.Termination

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AtomicLoadOrdering
- AtomicStoreOrdering
- AtomicUpdateOrdering
- AutoreleasingUnsafeMutablePointer
- Bool
- Character
- ClosedRange

  Conforms when `Bound` conforms to `Comparable`.

- ClosedRange.Index

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- CodingUserInfoKey
- CollectionDifference

  Conforms when `ChangeElement` conforms to `Equatable`.

- CollectionDifference.Change

  Conforms when `ChangeElement` conforms to `Equatable`.

- CollectionDifference.Index

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Hashable`.

- ContinuousClock.Instant
- Dictionary

  Conforms when `Key` conforms to `Hashable` and `Value` conforms to `Equatable`.

- Dictionary.Index

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Keys

  Conforms when `Key` conforms to `Hashable`.

- DiscontiguousSlice

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- DiscontiguousSlice.Index

  Conforms when `Base` conforms to `Collection`.

- Double
- Duration
- Duration.TimeFormatStyle
- Duration.TimeFormatStyle.Attributed
- Duration.TimeFormatStyle.Pattern
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.Attributed
- Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
- Duration.UnitsFormatStyle.Unit
- Duration.UnitsFormatStyle.UnitWidth
- Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy
- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ExecuteDistributedTargetError.ErrorCode
- FlattenSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- Float
- Float16
- Float80
- FloatingPointClassification
- FloatingPointRoundingRule
- FloatingPointSign
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- JobPriority
- KeyPath
- LazyPrefixWhileSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Hashable`.

- LocalTestingActorID
- ManagedBufferPointer

  Conforms when `Header` conforms to `Copyable`, `Header` conforms to `Escapable`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- Mirror.DisplayStyle
- Never
- ObjectIdentifier
- ObservationRegistrar
- OpaquePointer
- Optional

  Conforms when `Wrapped` conforms to `Equatable`.

- Optional.Publisher

  Conforms when `Wrapped` conforms to `Equatable`.

- PartialKeyPath
- Range

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- RangeSet

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- ReferenceWritableKeyPath
- RegexRepetitionBehavior
- RegexSemanticLevel
- RegexWordBoundaryKind
- RemoteCallTarget
- Result

  Conforms when `Success` conforms to `Hashable`, `Failure` conforms to `Error`, and `Failure` conforms to `Hashable`.

- Result.Publisher

  Conforms when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

- ReversedCollection.Index

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Hashable`.

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

- Set.Index

  Conforms when `Element` conforms to `Hashable`.

- String
- String.Comparator
- String.Encoding
- String.Index
- String.IntentInputOptions.CapitalizationType
- String.IntentInputOptions.KeyboardType
- String.LocalizationValue
- String.LocalizationValue.Placeholder
- String.StandardComparator
- Substring
- SuspendingClock.Instant
- Task

  Conforms when `Success` conforms to `Copyable`, `Success` conforms to `Escapable`, `Success` conforms to `Sendable`, and `Failure` conforms to `Error`.

- TaskPriority
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- Unicode.CanonicalCombiningClass
- Unicode.GeneralCategory
- Unicode.NumericType
- Unicode.Scalar
- Unicode.UTF32
- UnicodeDecodingResult
- UnownedTaskExecutor
- UnsafeCurrentTask
- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawPointer
- WordPair
- WritableKeyPath

## See Also

### Equality and Ordering

protocol Comparable

A type that can be compared using the relational operators `=`, and `>`.

protocol Identifiable

A class of types whose instances hold the value of an entity with stable identity.

