

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  firstValue(matchingCategory:) 

Instance Method

# firstValue(matchingCategory:)

Finds the first tag matching the specified category and returns the value of the matching tag.

RealityKitSwiftiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func firstValue(matchingCategory category: CMTypedTag.Category) -> T? where T : Sendable
```

Available when `Element` inherits `CMTag`.

## Discussion

- category: The category to match.

