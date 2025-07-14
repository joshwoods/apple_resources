

- AppKit
- NSView
-  setFrameSize(\_:) 

Instance Method

# setFrameSize(\_:)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

macOS

``` source
@MainActor
func setFrameSize(_ newSize: NSSize)
```

## Parameters 

`newSize`  

An `NSSize` structure specifying the new height and width of the frame rectangle.

## Discussion

Changing the frame does not mark the view as needing to be displayed. Set the needsDisplay property to true when you want the view to be redisplayed.

Changing the frame size results in the posting of an frameDidChangeNotification to the default notification center if the view is configured to do so.

In macOS 10.4 and later, you can override this method to support content preservation during live resizing. In your overridden implementation, include some conditional code to be executed only during a live resize operation. Your code must invalidate any portions of your view that need to be redrawn.

## See Also

### Modifying the Frame Rectangle

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func setFrameOrigin(NSPoint)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

