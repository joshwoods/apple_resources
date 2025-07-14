

- UIKit
- UIPushBehavior
-  angle 

Instance Property

# angle

The angle, in radians, of the force vector for the behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var angle: CGFloat { get set }
```

## Discussion

The default angle is `0` radians, using standard UIKit geometry. To configure the force vector for a push behavior, set the magnitude property as well as the angle property.

Alternatively, you can express the direction of force by using *x* and *y* components with the pushDirection property. Whichever approach you use, the alternate, equivalent values update automatically.

## See Also

### Configuring a push behavior

func setAngle(CGFloat, magnitude: CGFloat)

Sets the angle and magnitude of the force vector for the behavior.

var magnitude: CGFloat

The magnitude of the force vector for the push behavior.

var mode: UIPushBehavior.Mode

Returns the force mode for the push behavior.

func setTargetOffsetFromCenter(UIOffset, for: any UIDynamicItem)

Sets the offset, from the center of a dynamic item, at which to apply the push behavior’s force vector.

func targetOffsetFromCenter(for: any UIDynamicItem) -> UIOffset

Returns the offset, from the center of a dynamic item, at which the push behavior’s force vector is applied.

var pushDirection: CGVector

The direction of the force vector for the behavior, expressed as *x* and *y* components and using standard UIKit geometry.

