

- AppKit
- NSView
-  postsFrameChangedNotifications 

Instance Property

# postsFrameChangedNotifications

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

macOS

``` source
@MainActor
var postsFrameChangedNotifications: Bool { get set }
```

## Discussion

When the value of this property is true and the view’s frame rectangle changes to a new value, the view posts a frameDidChangeNotification to the default notification center. The notification is not posted when you set the frame rectangle to the value it already has. The default value of this property is true.

If the value of this property is currently false and and the frame has changed, changing the value to true causes the view to post a frameDidChangeNotification notification immediately. This happens even when there has been no net change in the view’s frame rectangle.

The following methods and properties can trigger a frame change notification:

- frame

- setFrameOrigin(_:)

- setFrameSize(_:)

- frameRotation

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

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

