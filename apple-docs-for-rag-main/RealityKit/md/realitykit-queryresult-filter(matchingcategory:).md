

- RealityKit
- QueryResult
-  filter(matchingCategory:) 

Instance Method

# filter(matchingCategory:)

Filters a sequence of tags based on matching the specified category. Returns the tags that match the specified category.

RealityKitSwiftiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func filter(matchingCategory category: CMTypedTag.Category) -> [CMTypedTag] where T : Sendable
```

Available when `Element` inherits `CMTag`.

## Discussion

- category: The category to match.

## See Also

### Excluding elements

func drop(while: (Self.Element) throws -> Bool) rethrows -> DropWhileSequence&lt;Self>

Returns a sequence by skipping the initial, consecutive elements that satisfy the given predicate.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

