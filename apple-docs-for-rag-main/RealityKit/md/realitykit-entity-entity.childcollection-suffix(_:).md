

- RealityKit
- Entity
- Entity.ChildCollection
-  suffix(\_:) 

Instance Method

# suffix(\_:)

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func suffix(_ maxLength: Int) -> Self.SubSequence
```

## Parameters 

`maxLength`  

The maximum number of elements to return. The value of `maxLength` must be greater than or equal to zero.

## Return Value

A subsequence terminating at the end of the collection with at most `maxLength` elements.

## Discussion

If the maximum length exceeds the number of elements in the collection, the result contains all the elements in the collection.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.suffix(2))
// Prints "[4, 5]"
print(numbers.suffix(10))
// Prints "[1, 2, 3, 4, 5]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

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

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

