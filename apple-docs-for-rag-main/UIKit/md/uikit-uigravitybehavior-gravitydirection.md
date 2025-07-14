

- UIKit
- UIGravityBehavior
-  gravityDirection 

Instance Property

# gravityDirection

The direction and magnitude of the gravitational force, expressed as a vector.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var gravityDirection: CGVector { get set }
```

## Discussion

The gravity vector is expressed as an *x, y* pair that represents the relative motion along the x and y axes of the reference view. A value of `1.0` corresponds to an acceleration of 1000 points / second², which is referred to as UIKit gravity and approximates the Earth’s own gravitational force. A value of `-1.0` represents the same amount of force, but in the opposite direction of the corresponding axis.

The default value of this property is the vector (`0.0, 1.0`), which represents a downward force in the reference view. Changing the angle or magnitude values also changes the value of this property.

## See Also

### Configuring a gravity behavior

var angle: CGFloat

The direction of the gravity vector, expressed in radians in the reference coordinate system.

var magnitude: CGFloat

The magnitude of the gravity vector.

func setAngle(CGFloat, magnitude: CGFloat)

Sets the angle and magnitude of the gravity vector for the behavior.

