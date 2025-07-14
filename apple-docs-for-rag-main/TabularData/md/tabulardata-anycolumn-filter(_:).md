

- TabularData
- AnyColumn
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func filter(_ isIncluded: (Self.Element) throws -> Bool) rethrows -> [Self.Element]
```

## Parameters 

`isIncluded`  

A closure that takes an element of the sequence as its argument and returns a Boolean value indicating whether the element should be included in the returned array.

## Return Value

An array of the elements that `isIncluded` allowed.

## Discussion

In this example, `filter(_:)` is used to include only names shorter than five characters.

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
let shortNames = cast.filter { $0.count 

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Generating Arrays

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

