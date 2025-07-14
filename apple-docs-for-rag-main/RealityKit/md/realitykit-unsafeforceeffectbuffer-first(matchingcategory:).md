

- RealityKit
- UnsafeForceEffectBuffer
-  first(matchingCategory:) 

Instance Method

# first(matchingCategory:)

Finds and returns the first tag matching the specified category.

RealityKitSwiftiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func first(matchingCategory category: CMTypedTag.Category) -> CMTypedTag? where T : Sendable
```

Available when `Element` inherits `CMTag`.

## Discussion

- category: The category to match.

