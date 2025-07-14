

- GameplayKit
- GKRandomDistribution
-  numberOfPossibleOutcomes 

Instance Property

# numberOfPossibleOutcomes

The number of unique values the distribution can generate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var numberOfPossibleOutcomes: Int { get }
```

## Discussion

When using the GKRandomDistribution directly, this property is determined by the lowestValue and highestValue properties according to the formula `number = highest - lowest + 1`. For example, in a distribution whose lowest value is 1 and highest value is 4, the nextInt() method can return `1`, `2`, `3`, or `4`, and the nextUniform() method can return `0.25`, `0.5`, `0.75`, or `1.0`, so the number of possible outcomes is 4.

Subclasses of GKRandomDistribution can alter the number of unique possible outcomes.

## See Also

### Working with Characteristics of a Distribution

var lowestValue: Int

The lowest value to be produced by the distribution.

var highestValue: Int

The highest value to be produced by the distribution.

