

- RealityKit
- Entity
- Entity.ChildCollection
-  prefix(while:) 

Instance Method

# prefix(while:)

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func prefix(while predicate: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be included or `false` if it should be excluded. Once the predicate returns `false` it will not be called again.

## Discussion

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Selecting entities

subscript(Int) -> Entity

Accesses the element at the specified position. (See `Collection.subscript`.)

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

