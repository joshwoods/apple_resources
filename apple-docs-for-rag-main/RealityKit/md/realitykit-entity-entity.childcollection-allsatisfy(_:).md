

- RealityKit
- Entity
- Entity.ChildCollection
-  allSatisfy(\_:) 

Instance Method

# allSatisfy(\_:)

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func allSatisfy(_ predicate: (Self.Element) throws -> Bool) rethrows -> Bool
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns a Boolean value that indicates whether the passed element satisfies a condition.

## Return Value

`true` if the sequence contains only elements that satisfy `predicate`; otherwise, `false`.

## Discussion

The following code uses this method to test whether all the names in an array have at least five characters:

```
let names = ["Sofia", "Camilla", "Martina", "Mateo", "Nicolás"]
let allHaveAtLeastFive = names.allSatisfy({ $0.count >= 5 })
// allHaveAtLeastFive == true
```

If the sequence is empty, this method returns `true`.

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Finding entities

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

var first: Self.Element?

The first element of the collection.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

