

- GameplayKit
- GKNoise
-  raiseToPower(\_:) 

Instance Method

# raiseToPower(\_:)

Replaces values in the noise field by exponentiating them with values from the specified noise object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func raiseToPower(_ noise: GKNoise)
```

## Parameters 

`noise`  

The noise object from which to use values as exponents.

## Discussion

Noise values are generally in the range \[-1.0, 1.0\], so exponentiating some points in a noise field can result in values outside the floating-point domain. Depending on the stylistic result you’re looking for, choose your base and exponent noises carefully or use other noise operations (such as the clamp(lowerBound:upperBound:) and remapValues(toCurveWithControlPoints:) methods) to conform the exponent noise to a specific range before using this method.

## See Also

### Applying Operations that Combine Noise

func add(GKNoise)

Replaces values in the noise field by adding them to values from the specified noise object.

func multiply(GKNoise)

Replaces values in the noise field by multiplying them with values from the specified noise object.

func maximum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

func minimum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

