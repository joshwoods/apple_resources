

- Swift
-  IndexingIterator 

Structure

# IndexingIterator

A type that iterates over a collection using its indices.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct IndexingIterator where Elements : Collection
```

## Overview

The `IndexingIterator` type is the default iterator for any collection that doesn’t declare its own. It acts as an iterator by using a collection’s indices to step over each value in the collection. Most collections in the standard library use `IndexingIterator` as their iterator.

By default, any custom collection type you create will inherit a `makeIterator()` method that returns an `IndexingIterator` instance, making it unnecessary to declare your own. When creating a custom collection type, add the minimal requirements of the `Collection` protocol: starting and ending indices and a subscript for accessing elements. With those elements defined, the inherited `makeIterator()` method satisfies the requirements of the `Sequence` protocol.

Here’s an example of a type that declares the minimal requirements for a collection. The `CollectionOfTwo` structure is a fixed-size collection that always holds two elements of a specific type.

```
struct CollectionOfTwo: Collection {
    let elements: (Element, Element)

    init(_ first: Element, _ second: Element) {
        self.elements = (first, second)
    }

    var startIndex: Int { return 0 }
    var endIndex: Int   { return 2 }

    subscript(index: Int) -> Element {
        switch index {
        case 0: return elements.0
        case 1: return elements.1
        default: fatalError("Index out of bounds.")
        }
    }

    func index(after i: Int) -> Int {
        precondition(i 

Because `CollectionOfTwo` doesn’t define its own `makeIterator()` method or `Iterator` associated type, it uses the default iterator type, `IndexingIterator`. This example shows how a `CollectionOfTwo` instance can be created holding the values of a point, and then iterated over using a `for`-`in` loop.

```
let point = CollectionOfTwo(15.0, 20.0)
for element in point {
    print(element)
}
// Prints "15.0"
// Prints "20.0"
```

## Topics

### Type Aliases

typealias SubSequence

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Elements` conforms to `Collection`.

- IteratorProtocol

  Conforms when `Elements` conforms to `Collection`.

- Sendable

  Conforms when `Elements` conforms to `Collection`, `Elements` conforms to `Sendable`, and `Elements.Index` conforms to `Sendable`.

- Sequence

  Conforms when `Elements` conforms to `Collection`.

## See Also

### Indices and Iterators

struct IteratorSequence

A sequence built around an iterator of type `Base`.

typealias EnumeratedIterator

typealias SetIterator

struct StrideThroughIterator

An iterator for a `StrideThrough` instance.

struct StrideToIterator

An iterator for a `StrideTo` instance.

