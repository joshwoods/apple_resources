

- UIKit
- UIPushBehavior
-  setAngle(\_:magnitude:) 

Instance Method

# setAngle(\_:magnitude:)

Sets the angle and magnitude of the force vector for the behavior.

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

The angle, in radians, of the force vector for the push behavior.

The default angle is `0` radians, using standard UIKit geometry.

`magnitude`  

The magnitude of the force vector for the push behavior.

The default magnitude is `nil`, equivalent to no force. A force vector with a magnitude of `1.0`, applied to a 100 point x 100 point view whose density value is `1.0`, results in view acceleration of 100 points / second².

Setting the magnitude parameter to a negative value reverses the direction of the force.

## Discussion

Whether you express a push behavior’s force direction in terms of radian angle or with *x*, *y* components, the alternate, equivalent values update automatically.

## See Also

### Configuring a push behavior

var angle: CGFloat

The angle, in radians, of the force vector for the behavior.

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

