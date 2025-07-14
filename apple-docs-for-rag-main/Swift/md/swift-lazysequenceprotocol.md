

- Swift
-  LazySequenceProtocol 

Protocol

# LazySequenceProtocol

A sequence on which normally-eager sequence operations are implemented lazily.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol LazySequenceProtocol : Sequence
```

## Overview

Lazy sequences can be used to avoid needless storage allocation and computation, because they use an underlying sequence for storage and compute their elements on demand. For example, `doubled` in this code sample is a sequence containing the values `2`, `4`, and `6`.

```
let doubled = [1, 2, 3].lazy.map { $0 * 2 }
```

Each time an element of the lazy sequence `doubled` is accessed, the closure accesses and transforms an element of the underlying array.

Sequence operations that take closure arguments, such as `map(_:)` and `filter(_:)`, are normally eager: They use the closure immediately and return a new array. When you use the `lazy` property, you give the standard library explicit permission to store the closure and the sequence in the result, and defer computation until it is needed.

## Adding New Lazy Operations

To add a new lazy sequence operation, extend this protocol with a method that returns a lazy wrapper that itself conforms to `LazySequenceProtocol`. For example, an eager `scan(_:_:)` method is defined as follows:

```
extension Sequence {
    /// Returns an array containing the results of
    ///
    ///   p.reduce(initial, nextPartialResult)
    ///
    /// for each prefix `p` of `self`, in order from shortest to
    /// longest. For example:
    ///
    ///     (1..(
        _ initial: Result,
        _ nextPartialResult: (Result, Element) -> Result
    ) -> [Result] {
        var result = [initial]
        for x in self {
            result.append(nextPartialResult(result.last!, x))
        }
        return result
    }
}
```

You can build a sequence type that lazily computes the elements in the result of a scan:

```
struct LazyScanSequence
    : LazySequenceProtocol
{
    let initial: Result
    let base: Base
    let nextPartialResult:
        (Result, Base.Element) -> Result

    struct Iterator: IteratorProtocol {
        var base: Base.Iterator
        var nextElement: Result?
        let nextPartialResult:
            (Result, Base.Element) -> Result

        mutating func next() -> Result? {
            return nextElement.map { result in
                nextElement = base.next().map {
                    nextPartialResult(result, $0)
                }
                return result
            }
        }
    }

    func makeIterator() -> Iterator {
        return Iterator(
            base: base.makeIterator(),
            nextElement: initial as Result?,
            nextPartialResult: nextPartialResult)
    }
}
```

Finally, you can give all lazy sequences a lazy `scan(_:_:)` method:

```
extension LazySequenceProtocol {
    func scan(
        _ initial: Result,
        _ nextPartialResult: @escaping (Result, Element) -> Result
    ) -> LazyScanSequence {
        return LazyScanSequence(
            initial: initial, base: self, nextPartialResult: nextPartialResult)
    }
}
```

With this type and extension method, you can call `.lazy.scan(_:_:)` on any sequence to create a lazily computed scan. The resulting `LazyScanSequence` is itself lazy, too, so further sequence operations also defer computation.

The explicit permission to implement operations lazily applies only in contexts where the sequence is statically known to conform to `LazySequenceProtocol`. In the following example, because the extension applies only to `Sequence`, side-effects such as the accumulation of `result` are never unexpectedly dropped or deferred:

```
extension Sequence where Element == Int {
    func sum() -> Int {
        var result = 0
        _ = self.map { result += $0 }
        return result
    }
}
```

Don’t actually use `map` for this purpose, however, because it creates and discards the resulting array. Instead, use `reduce` for summing operations, or `forEach` or a `for`-`in` loop for operations with side effects.

## Topics

### Associated Types

associatedtype Elements : Sequence = Self

A `Sequence` that can contain the same elements as this one, possibly with a simpler type.

**Required**

### Instance Properties

var elements: Self.Elements

A sequence containing the same elements as this one, possibly with a simpler type.

**Required** Default implementation provided.

var lazy: Self.Elements

var lazy: LazySequence&lt;Self.Elements>

### Instance Methods

func compactMap&lt;ElementOfResult>((Self.Elements.Element) -> ElementOfResult?) -> LazyMapSequence&lt;LazyFilterSequence&lt;LazyMapSequence&lt;Self.Elements, ElementOfResult?>>, ElementOfResult>

Returns the non-`nil` results of mapping the given transformation over this sequence.

func drop(while: (Self.Elements.Element) -> Bool) -> LazyDropWhileSequence&lt;Self.Elements>

Returns a lazy sequence that skips any initial elements that satisfy `predicate`.

func filter((Self.Elements.Element) -> Bool) -> LazyFilterSequence&lt;Self.Elements>

Returns the elements of `self` that satisfy `isIncluded`.

func flatMap&lt;ElementOfResult>((Self.Elements.Element) -> ElementOfResult?) -> LazyMapSequence&lt;LazyFilterSequence&lt;LazyMapSequence&lt;Self.Elements, ElementOfResult?>>, ElementOfResult>

Returns the non-`nil` results of mapping the given transformation over this sequence.

func flatMap&lt;SegmentOfResult>((Self.Elements.Element) -> SegmentOfResult) -> LazySequence&lt;FlattenSequence&lt;LazyMapSequence&lt;Self.Elements, SegmentOfResult>>>

Returns the concatenated results of mapping the given transformation over this sequence.

func joined() -> LazySequence&lt;FlattenSequence&lt;Self.Elements>>

Returns a lazy sequence that concatenates the elements of this sequence of sequences.

func map&lt;U>((Self.Element) -> U) -> LazyMapSequence&lt;Self.Elements, U>

Returns a `LazyMapSequence` over this `Sequence`. The elements of the result are computed lazily, each time they are read, by calling `transform` function on a base element.

func prefix(while: (Self.Elements.Element) -> Bool) -> LazyPrefixWhileSequence&lt;Self.Elements>

Returns a lazy sequence of the initial consecutive elements that satisfy `predicate`.

## Relationships

### Inherits From

- Sequence

### Inherited By

- LazyCollectionProtocol

### Conforming Types

- LazyDropWhileSequence

  Conforms when `Base` conforms to `Sequence`.

- LazyFilterSequence

  Conforms when `Base` conforms to `Collection`.

- LazyMapSequence

  Conforms when `Base` conforms to `Sequence`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyPrefixWhileSequence

  Conforms when `Base` conforms to `Collection`.

- LazySequence

  Conforms when `Base` conforms to `Collection`.

- ReversedCollection

  Conforms when `Base` conforms to `BidirectionalCollection` and `LazySequenceProtocol`.

- Slice

  Conforms when `Base` conforms to `Collection` and `LazySequenceProtocol`.

## See Also

### Lazy Collections

protocol LazyCollectionProtocol

