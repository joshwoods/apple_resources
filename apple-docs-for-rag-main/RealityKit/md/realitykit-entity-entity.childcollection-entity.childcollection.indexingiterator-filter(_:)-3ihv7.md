

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
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

func filter(Predicate&lt;Self.Element>) throws -> [Self.Element]

func prefix(Int) -> PrefixSequence&lt;Self>

Returns a sequence, up to the specified maximum length, containing the initial elements of the sequence.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns a sequence containing the initial, consecutive elements that satisfy the given predicate.

func suffix(Int) -> [Self.Element]

Returns a subsequence, up to the given maximum length, containing the final elements of the sequence.

