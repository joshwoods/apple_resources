

- UIKit
- UIPushBehavior
-  targetOffsetFromCenter(for:) 

Instance Method

# targetOffsetFromCenter(for:)

Returns the offset, from the center of a dynamic item, at which the push behavior’s force vector is applied.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func targetOffsetFromCenter(for item: any UIDynamicItem) -> UIOffset
```

## Parameters 

`item`  

The dynamic item for which you’re retrieving the target offset.

## Return Value

The offset, from the center of the dynamic item, at which the push behavior’s force vector is applied. If you haven’t set a target offset, returns the center of the dynamic item.

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

func setTargetOffsetFromCenter(UIOffset, for: any UIDynamicItem)

Sets the offset, from the center of a dynamic item, at which to apply the push behavior’s force vector.

var pushDirection: CGVector

The direction of the force vector for the behavior, expressed as *x* and *y* components and using standard UIKit geometry.

