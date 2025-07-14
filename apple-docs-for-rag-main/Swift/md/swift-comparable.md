

- Swift
-  Comparable 

Protocol

# Comparable

A type that can be compared using the relational operators `=`, and `>`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Comparable : Equatable
```

## Overview

The `Comparable` protocol is used for types that have an inherent order, such as numbers and strings. Many types in the standard library already conform to the `Comparable` protocol. Add `Comparable` conformance to your own custom types when you want to be able to compare instances using relational operators or use standard library methods that are designed for `Comparable` types.

The most familiar use of relational operators is to compare numbers, as in the following example:

```
let currentTemp = 73

if currentTemp >= 90 {
    print("It's a scorcher!")
} else if currentTemp 

You can use special versions of some sequence and collection operations when working with a `Comparable` type. For example, if your array’s elements conform to `Comparable`, you can call the `sort()` method without using arguments to sort the elements of your array in ascending order.

```
var measurements = [1.1, 1.5, 2.9, 1.2, 1.5, 1.3, 1.2]
measurements.sort()
print(measurements)
// Prints "[1.1, 1.2, 1.2, 1.3, 1.5, 1.5, 2.9]"
```

# Conforming to the Comparable Protocol

Types with Comparable conformance implement the less-than operator (``, `=` with instances of your type without any further code.

As an example, here’s an implementation of a `Date` structure that stores the year, month, and day of a date:

```
struct Date {
    let year: Int
    let month: Int
    let day: Int
}
```

To add `Comparable` conformance to `Date`, first declare conformance to `Comparable` and implement the `

```
extension Date: Comparable {
    static func  Bool {
        if lhs.year != rhs.year {
            return lhs.year 

This function uses the least specific nonmatching property of the date to determine the result of the comparison. For example, if the two `year` properties are equal but the two `month` properties are not, the date with the lesser value for `month` is the lesser of the two dates.

Next, implement the `==` operator function, the requirement inherited from the `Equatable` protocol.

```
    static func == (lhs: Date, rhs: Date) -> Bool {
        return lhs.year == rhs.year && lhs.month == rhs.month
            && lhs.day == rhs.day
    }
}
```

Two `Date` instances are equal if each of their corresponding properties is equal.

Now that `Date` conforms to `Comparable`, you can compare instances of the type with any of the relational operators. The following example compares the date of the first moon landing with the release of David Bowie’s song “Space Oddity”:

```
let spaceOddity = Date(year: 1969, month: 7, day: 11)   // July 11, 1969
let moonLanding = Date(year: 1969, month: 7, day: 20)   // July 20, 1969
if moonLanding > spaceOddity {
    print("Major Tom stepped through the door first.")
} else {
    print("David Bowie was following in Neil Armstrong's footsteps.")
}
// Prints "Major Tom stepped through the door first."
```

Note that the `>` operator provided by the standard library is used in this example, not the `

## Topics

### Range Expressions

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

### Tuple Comparison

Compare tuples of between two and six `Comparable` elements using these comparative operators.

func &lt; ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt;= ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func > ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func >= ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

func >= &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

func >= &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

func >= &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

func >= &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

func >= &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

### Operators

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

**Required** Default implementations provided.

static func &lt; (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

**Required** Default implementations provided.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

**Required** Default implementations provided.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

**Required** Default implementations provided.

## Relationships

### Inherits From

- Equatable

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- DurationProtocol
- FixedWidthInteger
- FloatingPoint
- InstantProtocol
- SignedInteger
- Strideable
- StringProtocol
- UnsignedInteger

### Conforming Types

- AnyIndex
- AutoreleasingUnsafeMutablePointer
- Character
- ClosedRange.Index

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- CollectionDifference.Index

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- ContinuousClock.Instant
- Dictionary.Index

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- DiscontiguousSlice.Index

  Conforms when `Base` conforms to `Collection`.

- Double
- Duration
- FlattenSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- JobPriority
- LazyPrefixWhileSequence.Index

  Conforms when `Base` conforms to `Collection`.

- Never
- ObjectIdentifier
- ReversedCollection.Index

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Set.Index

  Conforms when `Element` conforms to `Hashable`.

- String
- String.Index
- Substring
- SuspendingClock.Instant
- TaskPriority
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- Unicode.CanonicalCombiningClass
- Unicode.Scalar
- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawPointer
- WordPair

## See Also

### Equality and Ordering

protocol Equatable

A type that can be compared for value equality.

protocol Identifiable

A class of types whose instances hold the value of an entity with stable identity.

