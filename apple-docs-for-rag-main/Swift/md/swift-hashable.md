

- Swift
-  Hashable 

Protocol

# Hashable

A type that can be hashed into a `Hasher` to produce an integer hash value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Hashable : Equatable
```

## Mentioned in 

Adopting Common Protocols

## Overview

You can use any type that conforms to the `Hashable` protocol in a set or as a dictionary key. Many types in the standard library conform to `Hashable`: Strings, integers, floating-point and Boolean values, and even sets are hashable by default. Some other types, such as optionals, arrays and ranges automatically become hashable when their type arguments implement the same.

Your own custom types can be hashable as well. When you define an enumeration without associated values, it gains `Hashable` conformance automatically, and you can add `Hashable` conformance to your other custom types by implementing the `hash(into:)` method. For structs whose stored properties are all `Hashable`, and for enum types that have all-`Hashable` associated values, the compiler is able to provide an implementation of `hash(into:)` automatically.

Hashing a value means feeding its essential components into a hash function, represented by the `Hasher` type. Essential components are those that contribute to the type’s implementation of `Equatable`. Two instances that are equal must feed the same values to `Hasher` in `hash(into:)`, in the same order.

# Conforming to the Hashable Protocol

To use your own custom type in a set or as the key type of a dictionary, add `Hashable` conformance to your type. The `Hashable` protocol inherits from the `Equatable` protocol, so you must also satisfy that protocol’s requirements.

The compiler automatically synthesizes your custom type’s `Hashable` and requirements when you declare `Hashable` conformance in the type’s original declaration and your type meets these criteria:

- For a `struct`, all its stored properties must conform to `Hashable`.

- For an `enum`, all its associated values must conform to `Hashable`. (An `enum` without associated values has `Hashable` conformance even without the declaration.)

To customize your type’s `Hashable` conformance, to adopt `Hashable` in a type that doesn’t meet the criteria listed above, or to extend an existing type to conform to `Hashable`, implement the `hash(into:)` method in your custom type.

In your `hash(into:)` implementation, call `combine(_:)` on the provided `Hasher` instance with the essential components of your type. To ensure that your type meets the semantic requirements of the `Hashable` and `Equatable` protocols, it’s a good idea to also customize your type’s `Equatable` conformance to match.

As an example, consider a `GridPoint` type that describes a location in a grid of buttons. Here’s the initial declaration of the `GridPoint` type:

```
/// A point in an x-y coordinate system.
struct GridPoint {
    var x: Int
    var y: Int
}
```

You’d like to create a set of the grid points where a user has already tapped. Because the `GridPoint` type is not hashable yet, it can’t be used in a set. To add `Hashable` conformance, provide an `==` operator function and implement the `hash(into:)` method.

```
extension GridPoint: Hashable {
    static func == (lhs: GridPoint, rhs: GridPoint) -> Bool {
        return lhs.x == rhs.x && lhs.y == rhs.y
    }

    func hash(into hasher: inout Hasher) {
        hasher.combine(x)
        hasher.combine(y)
    }
}
```

The `hash(into:)` method in this example feeds the grid point’s `x` and `y` properties into the provided hasher. These properties are the same ones used to test for equality in the `==` operator function.

Now that `GridPoint` conforms to the `Hashable` protocol, you can create a set of previously tapped grid points.

```
var tappedPoints: Set = [GridPoint(x: 2, y: 3), GridPoint(x: 4, y: 1)]
let nextTap = GridPoint(x: 0, y: 1)
if tappedPoints.contains(nextTap) {
    print("Already tapped at (\(nextTap.x), \(nextTap.y)).")
} else {
    tappedPoints.insert(nextTap)
    print("New tap detected at (\(nextTap.x), \(nextTap.y)).")
}
// Prints "New tap detected at (0, 1).")
```

## Topics

### Providing a Hash Value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

**Required** Default implementations provided.

### Deprecated

var hashValue: Int

The hash value.

**Required**

## Relationships

### Inherits From

- Equatable

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- DistributedActor
- FixedWidthInteger
- FloatingPoint
- InstantProtocol
- SIMD
- SignedInteger
- StringProtocol
- UnsignedInteger

### Conforming Types

- AnyHashable
- AnyKeyPath
- Array

  Conforms when `Element` conforms to `Hashable`.

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

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- ClosedRange.Index

  Conforms when `Bound` conforms to `Hashable`, `Bound` conforms to `Strideable`, and `Bound.Stride` conforms to `SignedInteger`.

- CodingUserInfoKey
- CollectionDifference

  Conforms when `ChangeElement` conforms to `Hashable`.

- CollectionDifference.Change

  Conforms when `ChangeElement` conforms to `Hashable`.

- CollectionDifference.Index

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Hashable`.

- ContinuousClock.Instant
- Dictionary

  Conforms when `Key` conforms to `Hashable` and `Value` conforms to `Hashable`.

- Dictionary.Index

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- DiscontiguousSlice

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- DiscontiguousSlice.Index

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Hashable`.

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
- ExecuteDistributedTargetError.ErrorCode
- FlattenSequence.Index

  Conforms when `Base` conforms to `Collection`, `Base.Element` conforms to `Collection`, `Base.Index` conforms to `Hashable`, and `Base.Element.Index` conforms to `Hashable`.

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
- KeyPath
- LazyPrefixWhileSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Hashable`.

- LocalTestingActorID
- Mirror.DisplayStyle
- Never
- ObjectIdentifier
- ObservationRegistrar
- OpaquePointer
- Optional

  Conforms when `Wrapped` conforms to `Hashable`.

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
- String.LocalizationValue.Placeholder
- String.StandardComparator
- Substring
- SuspendingClock.Instant
- Task

  Conforms when `Success` conforms to `Copyable`, `Success` conforms to `Escapable`, `Success` conforms to `Sendable`, and `Failure` conforms to `Error`.

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

### Sets and Dictionaries

struct Hasher

The universal hash function used by `Set` and `Dictionary`.

