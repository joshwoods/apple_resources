

- RealityKit
- CharacterControllerComponent
-  skinWidth 

Instance Property

# skinWidth

An added tolerance around the character capsule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var skinWidth: Float
```

## Discussion

A small skin, known as the *contact offset*, is maintained around the controller’s volume to avoid rounding and precision issues with collision detection. Specify this value relative to the entity’s coordinate system.

## See Also

### Configuring a character

var height: Float

The capsule height.

var radius: Float

The capsule radius.

var slopeLimit: Float

The slope limit expressed as a limit angle in radians.

var stepLimit: Float

The maximum obstacle height that the controller can move over.

var upVector: SIMD3&lt;Float>

The y-axis direction relative to the physics origin.

