

- GameplayKit
- GKNoise
-  displaceWithNoises(x:y:z:) 

Instance Method

# displaceWithNoises(x:y:z:)

Replaces values in the noise field by shifting each value along a vector whose x-, y-, and z-components are based on the specified noise objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func displaceWithNoises(
    x xDisplacementNoise: GKNoise,
    y yDisplacementNoise: GKNoise,
    z zDisplacementNoise: GKNoise
)
```

## Parameters 

`xDisplacementNoise`  

A noise object whose values determine the x-component of distortion applied to each value in this noise field.

`yDisplacementNoise`  

A noise object whose values determine the y-component of distortion applied to each value in this noise field.

`zDisplacementNoise`  

A noise object whose values determine the z-component of distortion applied to each value in this noise field.

## Discussion

For each position in the noise field, this method first constructs a vector by sampling from the same position in the `xDisplacementNoise`, `yDisplacementNoise`, and `zDisplacementNoise` noise objects. Then this method uses that vector to shift the location of the noise value at that position. By applying different types of noise to each parameter, you can create different kinds of distortion effects. For example, passing GKCylindersNoiseSource output to one parameter and GKConstantNoiseSource to the other two, you can add horizontal, vertical, or transverse waves to the noise.

## See Also

### Applying Operations that Distort Noise

func applyTurbulence(frequency: Double, power: Double, roughness: Int32, seed: Int32)

Replaces values in the noise field by applying a randomized distortion effect.

