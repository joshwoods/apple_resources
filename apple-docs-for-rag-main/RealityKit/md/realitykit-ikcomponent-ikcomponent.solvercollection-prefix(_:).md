

- RealityKit
- IKComponent
- IKComponent.SolverCollection
-  prefix(\_:) 

Instance Method

# prefix(\_:)

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func prefix(_ maxLength: Int) -> Self.SubSequence
```

## Parameters 

`maxLength`  

The maximum number of elements to return. `maxLength` must be greater than or equal to zero.

## Return Value

A subsequence starting at the beginning of this collection with at most `maxLength` elements.

## Discussion

If the maximum length exceeds the number of elements in the collection, the result contains all the elements in the collection.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.prefix(2))
// Prints "[1, 2]"
print(numbers.prefix(10))
// Prints "[1, 2, 3, 4, 5]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the number of elements to select from the beginning of the collection.

