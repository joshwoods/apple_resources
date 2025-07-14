

- GameplayKit
- GKRandomDistribution
-  nextBool() 

Instance Method

# nextBool()

Generates and returns a new random Boolean value within the characteristics of the distribution.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextBool() -> Bool
```

## Return Value

A random Boolean value.

## Discussion

When using the GKRandomDistribution class directly, generated Boolean values are uniform—any call to this method has an equal chance of returning true or false. Subclasses of GKRandomDistribution can alter the relative probability of generating either value.

## See Also

### Generating Random Numbers

func nextInt() -> Int

Generates and returns a new random integer within the bounds of the distribution.

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer within the bounds of the distribution and less than the specified limit.

func nextUniform() -> Float

Generates and returns a new random floating-point value within the characteristics of the distribution.

