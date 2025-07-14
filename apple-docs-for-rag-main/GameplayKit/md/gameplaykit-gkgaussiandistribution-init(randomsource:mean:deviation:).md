

- GameplayKit
- GKGaussianDistribution
-  init(randomSource:mean:deviation:) 

Initializer

# init(randomSource:mean:deviation:)

Initializes a Gaussian random distribution with the specified mean and deviation, using the specified source randomizer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    randomSource source: any GKRandom,
    mean: Float,
    deviation: Float
)
```

## Parameters 

`source`  

A randomizer that produces raw random values for use by the distribution. A randomizer is any object implementing the GKRandom protocol, which can be a random source algorithm such as the GKARC4RandomSource class or another random distribution.

`mean`  

The mean value of the distribution (also called the *expected value* or *median*).

`deviation`  

The standard deviation of the distribution (also called *sigma*).

## Return Value

A new random distribution.

## Discussion

Using this initializer creates a Gaussian distribution whose range is determined by the specified `mean` and `deviation` values. The lowestValue property of the newly created distribution is set to three deviations below the mean (`lowest = mean - 3 * deviation`) and the highestValue property is set to three deviations above the mean (`highest = mean + 3 * deviation`).

A random distribution works by mapping the values produced by the `source` randomizer to the range and characteristics specified by the distribution. Multiple distributions can share the same source, with the side effect that retrieving a random value through one distribution affects the sequence of random numbers produced by the source.

## See Also

### Creating a Random Distribution

init(randomSource: any GKRandom, lowestValue: Int, highestValue: Int)

Initializes a Gaussian random distribution with the specified lower and upper bounds, using the specified source randomizer.

