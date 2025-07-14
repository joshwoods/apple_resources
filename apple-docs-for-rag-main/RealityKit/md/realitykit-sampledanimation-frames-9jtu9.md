

- RealityKit
- SampledAnimation
-  frames 

Instance Property

# frames

An array of weights in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var frames: [BlendShapeWeights] { get set }
```

Available when `Value` is `BlendShapeWeights`.

## Discussion

This array contains sequential values for the animated property when bindTarget is an array of weights.

