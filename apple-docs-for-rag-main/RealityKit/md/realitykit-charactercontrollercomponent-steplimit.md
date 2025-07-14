

- RealityKit
- CharacterControllerComponent
-  stepLimit 

Instance Property

# stepLimit

The maximum obstacle height that the controller can move over.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var stepLimit: Float
```

## Discussion

Specify this value relative to the entity’s coordinate system.

Changing this value after the CharacterControllerComponent has been created and added to Entity has no effect.

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

var upVector: SIMD3&lt;Float>

The y-axis direction relative to the physics origin.

