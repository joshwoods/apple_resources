

- Swift
-  Set 

Structure

# Set

An unordered collection of unique elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Set where Element : Hashable
```

## Overview

You use a set instead of an array when you need to test efficiently for membership and you aren’t concerned with the order of the elements in the collection, or when you need to ensure that each element appears only once in a collection.

You can create a set with any element type that conforms to the `Hashable` protocol. By default, most types in the standard library are hashable, including strings, numeric and Boolean types, enumeration cases without associated values, and even sets themselves.

Swift makes it as easy to create a new set as to create a new array. Simply assign an array literal to a variable or constant with the `Set` type specified.

```
let ingredients: Set = ["cocoa beans", "sugar", "cocoa butter", "salt"]
if ingredients.contains("sugar") {
    print("No thanks, too sweet.")
}
// Prints "No thanks, too sweet."
```

# Set Operations

Sets provide a suite of mathematical set operations. For example, you can efficiently test a set for membership of an element or check its intersection with another set:

- Use the `contains(_:)` method to test whether a set contains a specific element.

- Use the “equal to” operator (`==`) to test whether two sets contain the same elements.

- Use the `isSubset(of:)` method to test whether a set contains all the elements of another set or sequence.

- Use the `isSuperset(of:)` method to test whether all elements of a set are contained in another set or sequence.

- Use the `isStrictSubset(of:)` and `isStrictSuperset(of:)` methods to test whether a set is a subset or superset of, but not equal to, another set.

- Use the `isDisjoint(with:)` method to test whether a set has any elements in common with another set.

You can also combine, exclude, or subtract the elements of two sets:

- Use the `union(_:)` method to create a new set with the elements of a set and another set or sequence.

- Use the `intersection(_:)` method to create a new set with only the elements common to a set and another set or sequence.

- Use the `symmetricDifference(_:)` method to create a new set with the elements that are in either a set or another set or sequence, but not in both.

- Use the `subtracting(_:)` method to create a new set with the elements of a set that are not also in another set or sequence.

You can modify a set in place by using these methods’ mutating counterparts: `formUnion(_:)`, `formIntersection(_:)`, `formSymmetricDifference(_:)`, and `subtract(_:)`.

Set operations are not limited to use with other sets. Instead, you can perform set operations with another set, an array, or any other sequence type.

```
var primes: Set = [2, 3, 5, 7]

// Tests whether primes is a subset of a Range
print(primes.isSubset(of: 0..
let favoriteNumbers = [5, 7, 15, 21]
print(primes.intersection(favoriteNumbers))
// Prints "[5, 7]"
```

# Sequence and Collection Operations

In addition to the `Set` type’s set operations, you can use any nonmutating sequence or collection methods with a set.

```
if primes.isEmpty {
    print("No primes!")
} else {
    print("We have \(primes.count) primes.")
}
// Prints "We have 4 primes."

let primesSum = primes.reduce(0, +)
// 'primesSum' == 17

let primeStrings = primes.sorted().map(String.init)
// 'primeStrings' == ["2", "3", "5", "7"]
```

You can iterate through a set’s unordered elements with a `for`-`in` loop.

```
for number in primes {
    print(number)
}
// Prints "5"
// Prints "7"
// Prints "2"
// Prints "3"
```

Many sequence and collection operations return an array or a type-erasing collection wrapper instead of a set. To restore efficient set operations, create a new set from the result.

```
let primesStrings = primes.map(String.init)
// 'primesStrings' is of type Array
let primesStringsSet = Set(primes.map(String.init))
// 'primesStringsSet' is of type Set
```

# Bridging Between Set and NSSet

You can bridge between `Set` and `NSSet` using the `as` operator. For bridging to be possible, the `Element` type of a set must be a class, an `@objc` protocol (a protocol imported from Objective-C or marked with the `@objc` attribute), or a type that bridges to a Foundation type.

Bridging from `Set` to `NSSet` always takes O(1) time and space. When the set’s `Element` type is neither a class nor an `@objc` protocol, any required bridging of elements occurs at the first access of each element, so the first operation that uses the contents of the set (for example, a membership test) can take O(*n*).

Bridging from `NSSet` to `Set` first calls the `copy(with:)` method (`- copyWithZone:` in Objective-C) on the set to get an immutable copy and then performs additional Swift bookkeeping work that takes O(1) time. For instances of `NSSet` that are already immutable, `copy(with:)` returns the same set in constant time; otherwise, the copying performance is unspecified. The instances of `NSSet` and `Set` share buffer using the same copy-on-write optimization that is used when two instances of `Set` share buffer.

## Topics

### Creating a Set

In addition to using an array literal, you can also create a set using these initializers.

init()

Creates an empty set.

init(minimumCapacity: Int)

Creates an empty set with preallocated space for at least the specified number of elements.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init&lt;Source>(Source)

Creates a new set from a finite sequence of items.

### Inspecting a Set

var isEmpty: Bool

A Boolean value that indicates whether the set is empty.

var count: Int

The number of elements in the set.

var capacity: Int

The total number of elements that the set can contain without allocating new storage.

### Testing for Membership

func contains(Element) -> Bool

Returns a Boolean value that indicates whether the given element exists in the set.

### Adding Elements

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func insert&lt;ConcreteElement>(ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement)

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

func update&lt;ConcreteElement>(with: ConcreteElement) -> ConcreteElement?

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

### Removing Elements

func filter((Element) throws -> Bool) rethrows -> Set&lt;Element>

Returns a new set containing the elements of the set that satisfy the given predicate.

func remove(Element) -> Element?

Removes the specified element from the set.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func removeFirst() -> Element

Removes the first element of the set.

func remove(at: Set&lt;Element>.Index) -> Element

Removes the element at the given index of the set.

func removeAll(keepingCapacity: Bool)

Removes all members from the set.

### Combining Sets

func union&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements of both this set and the given sequence.

func formUnion&lt;S>(S)

Inserts the elements of the given sequence into the set.

func intersection(Set&lt;Element>) -> Set&lt;Element>

Returns a new set with the elements that are common to both this set and the given sequence.

func intersection&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements that are common to both this set and the given sequence.

func formIntersection&lt;S>(S)

Removes the elements of the set that aren’t also in the given sequence.

func symmetricDifference&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements that are either in this set or in the given sequence, but not in both.

func formSymmetricDifference(Set&lt;Element>)

Removes the elements of the set that are also in the given sequence and adds the members of the sequence that are not already in the set.

func formSymmetricDifference&lt;S>(S)

Replace this set with the elements contained in this set or the given set, but not both.

func subtract(Set&lt;Element>)

Removes the elements of the given set from this set.

func subtract&lt;S>(S)

Removes the elements of the given sequence from the set.

func subtracting(Set&lt;Element>) -> Set&lt;Element>

Returns a new set containing the elements of this set that do not occur in the given set.

func subtracting&lt;S>(S) -> Set&lt;Element>

Returns a new set containing the elements of this set that do not occur in the given sequence.

### Comparing Sets

static func == (Set&lt;Element>, Set&lt;Element>) -> Bool

Returns a Boolean value indicating whether two sets have equal elements.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func isSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a subset of the given set.

func isSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a subset of the given sequence.

func isStrictSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isStrictSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a superset of the given set.

func isSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given sequence.

func isStrictSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isStrictSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isDisjoint(with: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set has no members in common with the given set.

func isDisjoint&lt;S>(with: S) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given sequence.

### Accessing Individual Elements

var first: Self.Element?

The first element of the collection.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

### Finding Elements

subscript(Set&lt;Element>.Index) -> Element

Accesses the member at the given position.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func firstIndex(of: Element) -> Set&lt;Element>.Index?

Returns the index of the given element in the set, or `nil` if the element is not a member of the set.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

### Transforming a Set

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

### Iterating over a Set

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func makeIterator() -> Set&lt;Element>.Iterator

Returns an iterator over the members of the set.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

### Performing Collection Operations

Order Dependent Operations on Set

Perform order-dependent operations common to all collections, as implemented for `Set`.

### Encoding and Decoding

func encode(to: any Encoder) throws

Encodes the elements of this set into the given encoder in an unkeyed container.

init(from: any Decoder) throws

Creates a new set by decoding from the given decoder.

### Describing a Set

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var description: String

A string that represents the contents of the set.

var debugDescription: String

A string that represents the contents of the set, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the set.

### Reference Types

Use bridged reference types when you need reference semantics or Foundation-specific behavior.

class NSSet

An object representing a static, unordered collection of unique objects.

class NSMutableSet

An object representing a dynamic, unordered, uniquing collection, for use instead of a variable in cases that require reference semantics.

### Supporting Types

struct Index

The position of an element in a set.

struct Iterator

An iterator over the members of a `Set`.

### Infrequently Used Functionality

init(arrayLiteral: Element...)

Creates a set containing the elements of the given array literal.

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

### Type Aliases

typealias Specification

typealias UnderlyingSequence

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByArrayLiteral Implementations

Hashable Implementations

Sequence Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- CVarArg

  Conforms when `Element` conforms to `Hashable`.

- Collection

  Conforms when `Element` conforms to `Hashable`.

- Copyable

  Conforms when `Element` conforms to `Hashable`.

- CustomDebugStringConvertible

  Conforms when `Element` conforms to `Hashable`.

- CustomReflectable

  Conforms when `Element` conforms to `Hashable`.

- CustomStringConvertible

  Conforms when `Element` conforms to `Hashable`.

- Decodable

  Conforms when `Element` conforms to `Decodable` and `Hashable`.

- Encodable

  Conforms when `Element` conforms to `Encodable` and `Hashable`.

- Equatable

  Conforms when `Element` conforms to `Hashable`.

- ExpressibleByArrayLiteral

  Conforms when `Element` conforms to `Hashable`.

- Hashable

  Conforms when `Element` conforms to `Hashable`.

- Sendable

  Conforms when `Element` conforms to `Hashable` and `Sendable`.

- Sequence

  Conforms when `Element` conforms to `Hashable`.

- SetAlgebra

  Conforms when `Element` conforms to `Hashable`.

## See Also

### Sets

protocol OptionSet

A type that presents a mathematical set interface to a bit set.

