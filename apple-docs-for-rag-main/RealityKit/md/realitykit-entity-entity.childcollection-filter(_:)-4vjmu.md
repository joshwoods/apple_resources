

- RealityKit
- Entity
- Entity.ChildCollection
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

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

### Selecting entities

subscript(Int) -> Entity

Accesses the element at the specified position. (See `Collection.subscript`.)

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

