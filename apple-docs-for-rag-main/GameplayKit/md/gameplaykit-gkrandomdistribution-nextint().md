

- GameplayKit
- GKRandomDistribution
-  nextInt() 

Instance Method

# nextInt()

Generates and returns a new random integer within the bounds of the distribution.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextInt() -> Int
```

## Return Value

An integer in the range specified by the distribution’s lowestValue and highestValue properties (inclusive).

## Discussion

When using the GKRandomDistribution directly, generated numbers are uniform within this range. Subclasses of GKRandomDistribution can alter the relative probability of generating any particular number within the distribution’s range.

## See Also

### Generating Random Numbers

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer within the bounds of the distribution and less than the specified limit.

func nextUniform() -> Float

Generates and returns a new random floating-point value within the characteristics of the distribution.

func nextBool() -> Bool

Generates and returns a new random Boolean value within the characteristics of the distribution.

