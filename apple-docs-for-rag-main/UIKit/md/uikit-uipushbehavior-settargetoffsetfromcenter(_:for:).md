

- UIKit
- UIPushBehavior
-  setTargetOffsetFromCenter(\_:for:) 

Instance Method

# setTargetOffsetFromCenter(\_:for:)

Sets the offset, from the center of a dynamic item, at which to apply the push behavior’s force vector.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTargetOffsetFromCenter(
    _ o: UIOffset,
    for item: any UIDynamicItem
)
```

## Parameters 

`o`  

The offset, from the center of the dynamic item, at which to apply the push behavior’s force vector.

`item`  

The dynamic item for which you’re setting a target offset.

## Discussion

If you don’t set a target offset for a dynamic item, a push behavior’s force vector is applied at the item center.

## See Also

### Configuring a push behavior

func setAngle(CGFloat, magnitude: CGFloat)

Sets the angle and magnitude of the force vector for the behavior.

var angle: CGFloat

The angle, in radians, of the force vector for the behavior.

var magnitude: CGFloat

The magnitude of the force vector for the push behavior.

var mode: UIPushBehavior.Mode

Returns the force mode for the push behavior.

func targetOffsetFromCenter(for: any UIDynamicItem) -> UIOffset

Returns the offset, from the center of a dynamic item, at which the push behavior’s force vector is applied.

var pushDirection: CGVector

The direction of the force vector for the behavior, expressed as *x* and *y* components and using standard UIKit geometry.

