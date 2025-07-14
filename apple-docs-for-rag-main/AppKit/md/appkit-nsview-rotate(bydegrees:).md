

- AppKit
- NSView
-  rotate(byDegrees:) 

Instance Method

# rotate(byDegrees:)

Rotates the view’s bounds rectangle by a specified degree value around the origin of the coordinate system, (0.0, 0.0).

macOS

``` source
@MainActor
func rotate(byDegrees angle: CGFloat)
```

## Parameters 

`angle`  

A `float` value specifying the angle of rotation, in degrees.

## Discussion

See the boundsRotation method description for more information. This method neither redisplays the view nor marks it as needing display. You must do this yourself by calling the display() method or setting the needsDisplay property.

This method posts an boundsDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Related Documentation

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

var postsBoundsChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its bounds rectangle changes.

### Modifying the Coordinate System

func translateOrigin(to: NSPoint)

Translates the view’s coordinate system so that its origin moves to a new location.

func scaleUnitSquare(to: NSSize)

Scales the view’s coordinate system so that the unit square scales to the specified dimensions.

