

- AppKit
- NSView
-  frame 

Instance Property

# frame

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

macOS

``` source
@MainActor
var frame: NSRect { get set }
```

## Mentioned in 

Adopting the system text cursor in custom text views

## Discussion

Changing the value of this property repositions and resizes the view within the coordinate system of its superview. Changing the frame does not mark the view as needing to be displayed. Set the needsDisplay property to true when you want the view to be redisplayed.

If your view does not use a custom bounds rectangle, this method also sets the view’s bounds to match the size of the new frame. You can specify a custom bounds rectangle by changing the bounds property or by calling the setBoundsOrigin(_:) or setBoundsSize(_:) method explicitly. Once set, the view creates an internal transform to convert from frame coordinates to bounds coordinates. As long as the width-to-height ratio of the two coordinate systems remains the same, your content appears normal. If the ratios differ, your content may appear skewed.

The frame rectangle may be rotated relative to its superview’s coordinate system. For more information, see the frameRotation property.

Changing the value of this property results in the posting of an frameDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Related Documentation

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

### Modifying the Frame Rectangle

func setFrameOrigin(NSPoint)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

