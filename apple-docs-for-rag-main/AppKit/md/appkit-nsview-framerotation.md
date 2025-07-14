

- AppKit
- NSView
-  frameRotation 

Instance Property

# frameRotation

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

macOS

``` source
@MainActor
var frameRotation: CGFloat { get set }
```

## Discussion

Positive values indicate counterclockwise rotation. Negative values indicate clockwise rotation. Rotation is performed around the origin of the frame rectangle. Changing the value of this property does not mark the view as needing to be displayed. Set the needsDisplay property to true when you want the view to be redisplayed.

Changing the frame rotation value results in the posting of an frameDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Related Documentation

var boundsRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s bounds rectangle relative to its frame rectangle.

### Modifying the Frame Rectangle

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func setFrameOrigin(NSPoint)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

