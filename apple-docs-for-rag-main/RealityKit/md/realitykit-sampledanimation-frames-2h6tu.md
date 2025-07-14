

- RealityKit
- SampledAnimation
-  frames 

Instance Property

# frames

An array of quaternions in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var frames: [simd_quatf] { get set }
```

Available when `Value` is `simd_quatf`.

## Discussion

This array contains sequential values for the animated property when bindTarget is an array of quaternions.

## See Also

### Defining frames data

var frames: [JointTransforms]

An array of joint transforms in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

var frames: [Transform]

An array of transforms in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

var frames: [Double]

An array of double-precision values in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [Float]

An array of floating-point values in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD2&lt;Float>]

An array of floating-point pairs in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD3&lt;Float>]

An array of floating-point triplets in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD4&lt;Float>]

An array of floating-point quadruples in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

