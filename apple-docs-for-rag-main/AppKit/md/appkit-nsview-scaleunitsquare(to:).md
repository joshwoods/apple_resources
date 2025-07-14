

- AppKit
- NSView
-  scaleUnitSquare(to:) 

Instance Method

# scaleUnitSquare(to:)

Scales the view’s coordinate system so that the unit square scales to the specified dimensions.

macOS

``` source
@MainActor
func scaleUnitSquare(to newUnitSize: NSSize)
```

## Parameters 

`newUnitSize`  

An `NSSize` structure specifying the new unit size.

## Discussion

For example, a `newUnitSize` of (0.5, 1.0) causes the view’s horizontal coordinates to be halved, in turn doubling the width of its bounds rectangle. Note that scaling is performed from the origin of the coordinate system, (0.0, 0.0), not the origin of the bounds rectangle; as a result, both the origin and size of the bounds rectangle are changed. The frame rectangle remains unchanged.

This method does not redisplay the view or mark it as needing display. You must do this yourself by calling the display() method or setting the needsDisplay property.

This method posts an boundsDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Related Documentation

func setBoundsSize(NSSize)

Sets the size of the view’s bounds rectangle to specified dimensions, inversely scaling its coordinate system relative to its frame rectangle.

### Modifying the Coordinate System

func translateOrigin(to: NSPoint)

Translates the view’s coordinate system so that its origin moves to a new location.

func rotate(byDegrees: CGFloat)

Rotates the view’s bounds rectangle by a specified degree value around the origin of the coordinate system, (0.0, 0.0).

