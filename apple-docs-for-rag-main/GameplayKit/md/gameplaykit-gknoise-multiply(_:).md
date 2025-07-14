

- GameplayKit
- GKNoise
-  multiply(\_:) 

Instance Method

# multiply(\_:)

Replaces values in the noise field by multiplying them with values from the specified noise object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func multiply(_ noise: GKNoise)
```

## Parameters 

`noise`  

The noise object from which to multiply noise values.

## Discussion

Noise values are generally in the range \[-1.0, 1.0\], so multiplying typically results in moving values toward zero (in grayscale textures, a darkening effect).

## See Also

### Applying Operations that Combine Noise

func add(GKNoise)

Replaces values in the noise field by adding them to values from the specified noise object.

func raiseToPower(GKNoise)

Replaces values in the noise field by exponentiating them with values from the specified noise object.

func maximum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

func minimum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

