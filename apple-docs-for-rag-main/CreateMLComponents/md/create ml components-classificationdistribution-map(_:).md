

- Create ML Components
- ClassificationDistribution
-  map(\_:) 

Instance Method

# map(\_:)

Creates a new classification distribution by applying a transformation to every element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func map(_ transform: (Classification) throws -> Classification) rethrows -> ClassificationDistribution where T : Hashable
```

## Parameters 

`transform`  

A transformation closure.

## See Also

### Labeling and mapping

func topLabels(Int) -> [Label]

Computes the most likely labels in the classification set.

