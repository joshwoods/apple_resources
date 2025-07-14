

- RealityKit
- Entity
- Entity.ChildCollection
-  reversed() 

Instance Method

# reversed()

Returns an array containing the elements of this sequence in reverse order.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func reversed() -> [Self.Element]
```

## Return Value

An array containing the elements of this sequence in reverse order.

## Discussion

The sequence must be finite.

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Reordering entities

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

