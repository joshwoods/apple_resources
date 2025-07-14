

- RealityKit
- CharacterControllerComponent
-  slopeLimit 

Instance Property

# slopeLimit

The slope limit expressed as a limit angle in radians.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var slopeLimit: Float
```

## Discussion

This value represents the maximum slope that the character can move over. RealityKit applies this value to characters that are walking on static objects, but not when walking on kinematic or dynamic objects.

Changing this value after the CharacterControllerComponent has been created and added to Entity has no effect.

## See Also

### Configuring a character

var height: Float

The capsule height.

var radius: Float

The capsule radius.

var skinWidth: Float

An added tolerance around the character capsule.

var stepLimit: Float

The maximum obstacle height that the controller can move over.

var upVector: SIMD3&lt;Float>

The y-axis direction relative to the physics origin.

