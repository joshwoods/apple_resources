

- UIKit
- UIGravityBehavior
-  magnitude 

Instance Property

# magnitude

The magnitude of the gravity vector.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var magnitude: CGFloat { get set }
```

## Discussion

Modify this property when you want to change the magnitude of the gravity vector separately from the angle of that vector. A magnitude value of `1.0` represents an acceleration of 1000 points / second² at the specified angle, which roughly approximates the force of Earth’s gravity. The value in this property is tied to the value in the gravityDirection property, so changes in one affect the other.

The default value of this property is `1.0`.

Important

Setting the value of this property to `0.0` creates the vector (`0.0`, `0.0`) and resets the angle property to `0.0` radians. If you make subsequent changes to this property, also remember to update the angle property.

## See Also

### Configuring a gravity behavior

var gravityDirection: CGVector

The direction and magnitude of the gravitational force, expressed as a vector.

var angle: CGFloat

The direction of the gravity vector, expressed in radians in the reference coordinate system.

func setAngle(CGFloat, magnitude: CGFloat)

Sets the angle and magnitude of the gravity vector for the behavior.

