

- RealityKit
- Entity
- Entity.ChildCollection
-  randomElement(using:) 

Instance Method

# randomElement(using:)

Returns a random element of the collection, using the given generator as a source for randomness.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func randomElement(using generator: inout T) -> Self.Element? where T : RandomNumberGenerator
```

## Parameters 

`generator`  

The random number generator to use when choosing a random element.

## Return Value

A random element from the collection. If the collection is empty, the method returns `nil`.

## Discussion

Call `randomElement(using:)` to select a random element from an array or another collection when you are using a custom random number generator. This example picks a name at random from an array:

```
let names = ["Zoey", "Chloe", "Amani", "Amaia"]
let randomName = names.randomElement(using: &myGenerator)!
// randomName == "Amani"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

Note

The algorithm used to select a random element may change in a future version of Swift. If you’re passing a generator that results in the same sequence of elements each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

## See Also

### Finding entities

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

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

