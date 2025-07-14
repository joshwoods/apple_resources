

- Swift
- Dictionary
-  compactMap(\_:) 

Instance Method

# compactMap(\_:)

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compactMap(_ transform: (Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]
```

## Parameters 

`transform`  

A closure that accepts an element of this sequence as its argument and returns an optional value.

## Return Value

An array of the non-`nil` results of calling `transform` with each element of the sequence.

## Discussion

Use this method to receive an array of non-optional values when your transformation produces an optional value.

In this example, note the difference in the result of using `map` and `compactMap` with a transformation that returns an optional `Int` value.

```
let possibleNumbers = ["1", "2", "three", "///4///", "5"]

let mapped: [Int?] = possibleNumbers.map { str in Int(str) }
// [1, 2, nil, nil, 5]

let compactMapped: [Int] = possibleNumbers.compactMap { str in Int(str) }
// [1, 2, 5]
```

Complexity

O(*n*), where *n* is the length of this sequence.

## See Also

### Transforming a Dictionary

func mapValues&lt;T>((Value) throws -> T) rethrows -> Dictionary&lt;Key, T>

Returns a new dictionary containing the keys of this dictionary with the values transformed by the given closure.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func compactMapValues&lt;T>((Value) throws -> T?) rethrows -> Dictionary&lt;Key, T>

Returns a new dictionary containing only the key-value pairs that have non-`nil` values as the result of transformation by the given closure.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

