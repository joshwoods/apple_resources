

- UIKit
- UIGravityBehavior
-  setAngle(\_:magnitude:) 

Instance Method

# setAngle(\_:magnitude:)

Sets the angle and magnitude of the gravity vector for the behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setAngle(
    _ angle: CGFloat,
    magnitude: CGFloat
)
```

## Parameters 

`angle`  

The radian angle for the gravity vector, using standard UIKit geometry. Specify the value `pi / 2` to create a force that pulls items downward toward the bottom of the reference view.

`magnitude`  

The magnitude of the gravitational force. Specify `1.0` to get the standard UIKit gravity, which has an acceleration value of 1000 points / second².

## See Also

### Configuring a gravity behavior

var gravityDirection: CGVector

The direction and magnitude of the gravitational force, expressed as a vector.

var angle: CGFloat

The direction of the gravity vector, expressed in radians in the reference coordinate system.

var magnitude: CGFloat

The magnitude of the gravity vector.

