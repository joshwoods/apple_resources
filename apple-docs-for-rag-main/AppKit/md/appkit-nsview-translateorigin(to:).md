

- AppKit
- NSView
-  translateOrigin(to:) 

Instance Method

# translateOrigin(to:)

Translates the view’s coordinate system so that its origin moves to a new location.

macOS

``` source
@MainActor
func translateOrigin(to translation: NSPoint)
```

## Parameters 

`translation`  

A point that specifies the new origin.

## Discussion

In the process, the origin of the view’s bounds rectangle is shifted by (`–translation.x`, `–translation.y`). This method neither redisplays the view nor marks it as needing display. You must do this yourself by calling the display() method or setting the needsDisplay property.

Note the difference between this method and setting the bounds origin. Translation effectively moves the image inside the bounds rectangle, while setting the bounds origin effectively moves the rectangle over the image. The two are in a sense inverse, although translation is cumulative, and setting the bounds origin is absolute.

This method posts an boundsDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Related Documentation

func setBoundsOrigin(NSPoint)

Sets the origin of the view’s bounds rectangle to a specified point.

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

### Modifying the Coordinate System

func scaleUnitSquare(to: NSSize)

Scales the view’s coordinate system so that the unit square scales to the specified dimensions.

func rotate(byDegrees: CGFloat)

Rotates the view’s bounds rectangle by a specified degree value around the origin of the coordinate system, (0.0, 0.0).

