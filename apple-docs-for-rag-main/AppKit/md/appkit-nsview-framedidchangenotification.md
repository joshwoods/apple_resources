

- AppKit
- NSView
-  frameDidChangeNotification 

Type Property

# frameDidChangeNotification

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

macOS

``` source
class let frameDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSView` object whose frame rectangle has changed. This notification does not contain a `userInfo` dictionary.

The following methods can result in notification posting:

- frame

- setFrameOrigin(_:)

- frameRotation

- setFrameSize(_:)

## See Also

### Modifying the Frame Rectangle

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func setFrameOrigin(NSPoint)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

