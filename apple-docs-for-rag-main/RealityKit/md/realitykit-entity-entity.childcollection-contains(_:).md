

- RealityKit
- Entity
- Entity.ChildCollection
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the sequence contains the given element.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func contains(_ element: Self.Element) -> Bool
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`element`  

The element to find in the sequence.

## Return Value

`true` if the element was found in the sequence; otherwise, `false`.

## Discussion

This example checks to see whether a favorite actor is in an array storing a movie’s cast.

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
print(cast.contains("Marlon"))
// Prints "true"
print(cast.contains("James"))
// Prints "false"
```

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Finding entities

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

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

