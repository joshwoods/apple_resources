

- GameplayKit
- GKRandomDistribution
-  init(forDieWithSideCount:) 

Initializer

# init(forDieWithSideCount:)

Creates a random distribution equivalent to a die with the specified number of sides.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(forDieWithSideCount sideCount: Int)
```

## Parameters 

`sideCount`  

The count of sides for modeling a die; that is, the highest integer value for the random distribution to generate.

## Return Value

A uniform random distribution that produces values in the range `[1, sideCount]`.

## Discussion

Creating a random source with this method is equivalent to calling the init(randomSource:lowestValue:highestValue:) initializer, passing a new instance of the GKARC4RandomSource class for the `source` parameter, and passing 1 and `sideCount` for the `lowestValue` and `highestValue` parameters. Because the newly created distribution uses its own GKRandomSource instance, the random behavior of the distribution is independent from that of other randomizers.

## See Also

### Creating Specific Random Distributions

class func d6() -> Self

Creates a random distribution equivalent to a six-sided die.

class func d20() -> Self

Creates a random distribution equivalent to a twenty-sided die.

