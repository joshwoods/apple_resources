

- AppKit
- NSBox
-  setFrameFromContentFrame(\_:) 

Instance Method

# setFrameFromContentFrame(\_:)

Places the receiver so its content view lies on the specified frame.

macOS

``` source
@MainActor
func setFrameFromContentFrame(_ contentFrame: NSRect)
```

## Parameters 

`contentFrame`  

The rectangle specifying the frame of the box’s content view, reckoned in the coordinate system of the box’s superview. The box is marked for redisplay.

## See Also

### Related Documentation

var contentViewMargins: NSSize

The distances between the border and the content view.

var needsDisplay: Bool

A Boolean value that determines whether the view needs to be redrawn before being displayed.

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

### Sizing

func sizeToFit()

Resizes and moves the receiver’s content view so it just encloses its subviews.

