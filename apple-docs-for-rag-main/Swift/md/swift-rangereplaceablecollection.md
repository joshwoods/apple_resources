

- Swift
-  RangeReplaceableCollection 

Protocol

# RangeReplaceableCollection

A collection that supports replacement of an arbitrary subrange of elements with the elements of another collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol RangeReplaceableCollection : Collection where Self.SubSequence : RangeReplaceableCollection
```

## Overview

Range-replaceable collections provide operations that insert and remove elements. For example, you can add elements to an array of strings by calling any of the inserting or appending operations that the `RangeReplaceableCollection` protocol defines.

```
var bugs = ["Aphid", "Damselfly"]
bugs.append("Earwig")
bugs.insert(contentsOf: ["Bumblebee", "Cicada"], at: 1)
print(bugs)
// Prints "["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]"
```

Likewise, `RangeReplaceableCollection` types can remove one or more elements using a single operation.

```
bugs.removeLast()
bugs.removeSubrange(1...2)
print(bugs)
// Prints "["Aphid", "Damselfly"]"

bugs.removeAll()
print(bugs)
// Prints "[]"
```

Lastly, use the eponymous `replaceSubrange(_:with:)` method to replace a subrange of elements with the contents of another collection. Here, three elements in the middle of an array of integers are replaced by the five elements of a `Repeated` instance.

```
 var nums = [10, 20, 30, 40, 50]
 nums.replaceSubrange(1...3, with: repeatElement(1, count: 5))
 print(nums)
 // Prints "[10, 1, 1, 1, 1, 1, 50]"
```

# Conforming to the RangeReplaceableCollection Protocol

To add `RangeReplaceableCollection` conformance to your custom collection, add an empty initializer and the `replaceSubrange(_:with:)` method to your custom type. `RangeReplaceableCollection` provides default implementations of all its other methods using this initializer and method. For example, the `removeSubrange(_:)` method is implemented by calling `replaceSubrange(_:with:)` with an empty collection for the `newElements` parameter. You can override any of the protocol’s required methods to provide your own custom implementation.

## Topics

### Creating a New Collection

init()

Creates a new, empty collection.

**Required**

### Adding Elements

func insert&lt;S>(contentsOf: S, at: Self.Index)

Inserts the elements of a sequence into the collection at the specified position.

**Required** Default implementation provided.

### Operators

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of a collection and a sequence.

static func + &lt;Other>(Other, Self) -> Self

Creates a new collection by concatenating the elements of a sequence and a collection.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

### Associated Types

associatedtype SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

**Required**

### Initializers

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

**Required** Default implementation provided.

init(repeating: Self.Element, count: Int)

Creates a new collection containing the specified number of a single, repeated value.

**Required** Default implementation provided.

### Instance Methods

func append(Self.Element)

Adds an element to the end of the collection.

**Required** Default implementation provided.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

**Required** Default implementation provided.

func applying(CollectionDifference&lt;Self.Element>) -> Self?

Applies the given difference to this collection.

func filter((Self.Element) throws -> Bool) rethrows -> Self

Returns a new collection of the same type containing, in order, the elements of the original collection that satisfy the given predicate.

func insert(Self.Element, at: Self.Index)

Inserts a new element into the collection at the specified position.

**Required** Default implementation provided.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

**Required** Default implementation provided.

func remove(atOffsets: IndexSet)

Removes all the elements at the specified offsets from the collection.

func removeAll(keepingCapacity: Bool)

Removes all elements from the collection.

**Required** Default implementation provided.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

**Required** Default implementations provided.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

**Required** Default implementations provided.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

**Required** Default implementations provided.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the specified subrange of elements from the collection.

**Required** Default implementations provided.

func removeSubranges(RangeSet&lt;Self.Index>)

Removes the elements at the given indices.

func replace&lt;Output, Replacement>(some RegexComponent, maxReplacements: Int, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows

Replaces all occurrences of the sequence matching the given regex with a given collection.

func replace&lt;Replacement>(some RegexComponent, with: Replacement, maxReplacements: Int)

Replaces all occurrences of the sequence matching the given regex with a given collection.

func replace&lt;C, Replacement>(C, with: Replacement, maxReplacements: Int)

Replaces all occurrences of a target sequence with a given collection

func replace&lt;Output, Replacement>(maxReplacements: Int, content: () -> some RegexComponent, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows

Replaces all matches for the regex in this collection, using the given closures to create the replacement and the regex.

func replace&lt;Replacement>(with: Replacement, maxReplacements: Int, content: () -> some RegexComponent)

Replaces all matches for the regex in this collection, using the given closure to create the regex.

func replaceSubrange&lt;C>(Range&lt;Self.Index>, with: C)

Replaces the specified subrange of elements with the given collection.

**Required** Default implementation provided.

func replacing&lt;Output, Replacement>(some RegexComponent, maxReplacements: Int, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows -> Self

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another collection.

func replacing&lt;Output, Replacement>(some RegexComponent, subrange: Range&lt;Self.Index>, maxReplacements: Int, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows -> Self

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another regex match.

func replacing&lt;Replacement>(some RegexComponent, with: Replacement, maxReplacements: Int) -> Self

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another collection.

func replacing&lt;C, Replacement>(C, with: Replacement, maxReplacements: Int) -> Self

Returns a new collection in which all occurrences of a target sequence are replaced by another collection.

func replacing&lt;C, Replacement>(C, with: Replacement, subrange: Range&lt;Self.Index>, maxReplacements: Int) -> Self

Returns a new collection in which all occurrences of a target sequence are replaced by another collection.

func replacing&lt;Replacement>(some RegexComponent, with: Replacement, subrange: Range&lt;Self.Index>, maxReplacements: Int) -> Self

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another collection.

func replacing&lt;Output, Replacement>(maxReplacements: Int, content: () -> some RegexComponent, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows -> Self

Returns a new collection in which all matches for the regex are replaced, using the given closures to create the replacement and the regex.

func replacing&lt;Output, Replacement>(subrange: Range&lt;Self.Index>, maxReplacements: Int, content: () -> some RegexComponent, with: (Regex&lt;Output>.Match) throws -> Replacement) rethrows -> Self

Returns a new collection in which all matches for the regex are replaced, using the given closures to create the replacement and the regex.

func replacing&lt;Replacement>(with: Replacement, maxReplacements: Int, content: () -> some RegexComponent) -> Self

Returns a new collection in which all matches for the regex are replaced, using the given closure to create the regex.

func replacing&lt;Replacement>(with: Replacement, subrange: Range&lt;Self.Index>, maxReplacements: Int, content: () -> some RegexComponent) -> Self

Returns a new collection in which all matches for the regex are replaced, using the given closure to create the regex.

func reserveCapacity(Int)

Prepares the collection to store the specified number of elements, when doing so is appropriate for the underlying type.

**Required** Default implementation provided.

func trimPrefix(() -> some RegexComponent)

Removes the initial elements matching the regex from the start of this collection, if the initial elements match, using the given closure to create the regex.

func trimPrefix(some RegexComponent)

Removes the initial elements that matches the given regex.

func trimPrefix&lt;Prefix>(Prefix)

Removes `prefix` from the start of the collection.

func trimPrefix(while: (Self.Element) throws -> Bool) rethrows

### Subscripts

subscript(Self.Index) -> Self.Element

Accesses the element at the specified position.

**Required**

subscript(Range&lt;Self.Index>) -> Self.SubSequence

**Required**

## Relationships

### Inherits From

- Collection
- Sequence

### Conforming Types

- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Slice

  Conforms when `Base` conforms to `RangeReplaceableCollection`.

- String
- String.UnicodeScalarView
- Substring
- Substring.UnicodeScalarView

## See Also

### Collection Mutability

protocol MutableCollection

A collection that supports subscript assignment.

