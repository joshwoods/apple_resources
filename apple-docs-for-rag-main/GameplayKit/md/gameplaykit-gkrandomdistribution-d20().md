

- GameplayKit
- GKRandomDistribution
-  d20() 

Type Method

# d20()

Creates a random distribution equivalent to a twenty-sided die.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func d20() -> Self
```

## Return Value

A uniform random distribution that produces values in the range `[1, 20]`.

## Discussion

The newly created distribution uses its own GKRandomSource instance, so the random behavior of the distribution is independent from that of other randomizers.

## See Also

### Creating Specific Random Distributions

class func d6() -> Self

Creates a random distribution equivalent to a six-sided die.

convenience init(forDieWithSideCount: Int)

Creates a random distribution equivalent to a die with the specified number of sides.

