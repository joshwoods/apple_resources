

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  filter(\_:) 

Instance Method

# filter(\_:)

RealityKitSwiftiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func filter(_ predicate: Predicate) throws -> [Self.Element]
```

## See Also

### Selecting entities

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

func prefix(Int) -> PrefixSequence&lt;Self>

Returns a sequence, up to the specified maximum length, containing the initial elements of the sequence.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns a sequence containing the initial, consecutive elements that satisfy the given predicate.

func suffix(Int) -> [Self.Element]

Returns a subsequence, up to the given maximum length, containing the final elements of the sequence.

