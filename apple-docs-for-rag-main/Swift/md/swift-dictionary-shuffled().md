

- Swift
- Dictionary
-  shuffled() 

Instance Method

# shuffled()

Returns the elements of the sequence, shuffled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func shuffled() -> [Self.Element]
```

## Return Value

A shuffled array of this sequence’s elements.

## Discussion

For example, you can shuffle the numbers between `0` and `9` by calling the `shuffled()` method on that range:

```
let numbers = 0...9
let shuffledNumbers = numbers.shuffled()
// shuffledNumbers == [1, 7, 6, 2, 8, 9, 4, 3, 5, 0]
```

This method is equivalent to calling `shuffled(using:)`, passing in the system’s default random generator.

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Transforming a Dictionary

func mapValues&lt;T>((Value) throws -> T) rethrows -> Dictionary&lt;Key, T>

Returns a new dictionary containing the keys of this dictionary with the values transformed by the given closure.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func compactMapValues&lt;T>((Value) throws -> T?) rethrows -> Dictionary&lt;Key, T>

Returns a new dictionary containing only the key-value pairs that have non-`nil` values as the result of transformation by the given closure.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

