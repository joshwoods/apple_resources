

- RealityKit
- CharacterControllerComponent
-  upVector 

Instance Property

# upVector

The y-axis direction relative to the physics origin.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var upVector: SIMD3
```

## Discussion

Rotates the object so that the vertical height is along the up vector. Normalize and specify the vector in *physics space*, the coordinate system of the physics simulation.

## See Also

### Configuring a character

var height: Float

The capsule height.

var radius: Float

The capsule radius.

var skinWidth: Float

An added tolerance around the character capsule.

var slopeLimit: Float

The slope limit expressed as a limit angle in radians.

var stepLimit: Float

The maximum obstacle height that the controller can move over.

