

- Create ML
- MLDataTable
- MLDataTable.ColumnNames
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

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

