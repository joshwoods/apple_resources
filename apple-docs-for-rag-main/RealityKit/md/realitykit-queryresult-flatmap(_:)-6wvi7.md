

- RealityKit
- QueryResult
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func flatMap(_ transform: (Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element] where SegmentOfResult : Sequence
```

## Parameters 

`transform`  

A closure that accepts an element of this sequence as its argument and returns a sequence or collection.

## Return Value

The resulting flattened array.

## Discussion

Use this method to receive a single-level collection when your transformation produces a sequence or collection for each element.

In this example, note the difference in the result of using `map` and `flatMap` with a transformation that returns an array.

```
let numbers = [1, 2, 3, 4]

let mapped = numbers.map { Array(repeating: $0, count: $0) }
// [[1], [2, 2], [3, 3, 3], [4, 4, 4, 4]]

let flatMapped = numbers.flatMap { Array(repeating: $0, count: $0) }
// [1, 2, 2, 3, 3, 3, 4, 4, 4, 4]
```

In fact, `s.flatMap(transform)` is equivalent to `Array(s.map(transform).joined())`.

Complexity

O(*m* + *n*), where *n* is the length of this sequence and *m* is the length of the result.

## See Also

### Transforming a sequence

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

