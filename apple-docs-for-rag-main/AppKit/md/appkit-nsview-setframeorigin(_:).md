

- AppKit
- NSView
-  setFrameOrigin(\_:) 

Instance Method

# setFrameOrigin(\_:)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

macOS

``` source
@MainActor
func setFrameOrigin(_ newOrigin: NSPoint)
```

## Parameters 

`newOrigin`  

The point that is the new origin of the view’s frame.

## Discussion

Changing the frame does not mark the view as needing to be displayed. Set the needsDisplay property to true when you want the view to be redisplayed.

Changing the frame origin results in the posting of an frameDidChangeNotification to the default notification center if the view is configured to do so.

## See Also

### Modifying the Frame Rectangle

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

