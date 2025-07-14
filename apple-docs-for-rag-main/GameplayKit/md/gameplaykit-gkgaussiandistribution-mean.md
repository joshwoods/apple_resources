

- GameplayKit
- GKGaussianDistribution
-  mean 

Instance Property

# mean

The mean value of the distribution (also called the *expected value* or *median*).

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var mean: Float { get }
```

## Discussion

Random samplings from the distribution are most likely to result in the mean value, with other values increasingly far from the mean occurring with decreasing probability.

This property is read-only—its value is always the midpoint between the values of the inherited lowestValue and highestValue properties (`mean = (highest + lowest) / 2`).

## See Also

### Working with Characteristics of a Distribution

var deviation: Float

The standard deviation of the distribution (also called *sigma*).

