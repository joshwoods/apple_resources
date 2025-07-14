

- GameplayKit
- GKGaussianDistribution
-  init(randomSource:lowestValue:highestValue:) 

Initializer

# init(randomSource:lowestValue:highestValue:)

Initializes a Gaussian random distribution with the specified lower and upper bounds, using the specified source randomizer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    randomSource source: any GKRandom,
    lowestValue lowestInclusive: Int,
    highestValue highestInclusive: Int
)
```

## Parameters 

`source`  

A randomizer that produces raw random values for use by the distribution. A randomizer is any object implementing the GKRandom protocol, which can be a random source algorithm such as the GKARC4RandomSource class or another random distribution.

`lowestInclusive`  

The lowest value to be produced by the distribution.

`highestInclusive`  

The highest value to be produced by the distribution.

## Return Value

A new random distribution.

## Discussion

Using this initializer creates a Gaussian distribution centered within the specified range. The mean property is set to the midpoint between the `lowestInclusive` and `highestInclusive` parameters (`mean = (highest + lowest) / 2`), and the deviation property is set such that the highest and lowest values are each three deviations away from the mean (`deviation = (highest - lowest) / 6`). The mean and deviation properties can thus be floating-point values even if you use the distribution only to produce integers.

A random distribution works by mapping the values produced by the `source` randomizer to the range and characteristics specified by the distribution. Multiple distributions can share the same source, with the side effect that retrieving a random value through one distribution affects the sequence of random numbers produced by the source.

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Random Distribution

init(randomSource: any GKRandom, mean: Float, deviation: Float)

Initializes a Gaussian random distribution with the specified mean and deviation, using the specified source randomizer.

