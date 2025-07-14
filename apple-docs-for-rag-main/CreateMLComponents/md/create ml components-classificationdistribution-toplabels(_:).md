

- Create ML Components
- ClassificationDistribution
-  topLabels(\_:) 

Instance Method

# topLabels(\_:)

Computes the most likely labels in the classification set.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func topLabels(_ amount: Int) -> [Label]
```

## Parameters 

`amount`  

The number of top labels.

## Return Value

The labels with the highest probabilities.

## See Also

### Labeling and mapping

func map&lt;T>((Classification&lt;Label>) throws -> Classification&lt;T>) rethrows -> ClassificationDistribution&lt;T>

Creates a new classification distribution by applying a transformation to every element.

