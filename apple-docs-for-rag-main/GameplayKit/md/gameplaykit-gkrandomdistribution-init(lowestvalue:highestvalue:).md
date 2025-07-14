

- GameplayKit
- GKRandomDistribution
-  init(lowestValue:highestValue:) 

Initializer

# init(lowestValue:highestValue:)

Creates a random distribution with the specified lower and upper bounds, using the Arc4 randomizer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    lowestValue lowestInclusive: Int,
    highestValue highestInclusive: Int
)
```

## Parameters 

`lowestInclusive`  

The lowest value to be produced by the distribution.

`highestInclusive`  

The highest value to be produced by the distribution.

## Return Value

A new random distribution.

## Discussion

Creating a random source with this method is equivalent to calling the init(randomSource:lowestValue:highestValue:) initializer and passing a new instance of the GKARC4RandomSource class for the `source` parameter. Because the newly created distribution uses its own GKRandomSource instance, the random behavior of the distribution is independent from that of other randomizers.

## See Also

### Creating a Random Distribution

init(randomSource: any GKRandom, lowestValue: Int, highestValue: Int)

Initializes a uniform random distribution with the specified lower and upper bounds, using the specified source randomizer.

