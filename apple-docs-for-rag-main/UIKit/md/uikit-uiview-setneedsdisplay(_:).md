

- UIKit
- UIView
-  setNeedsDisplay(\_:) 

Instance Method

# setNeedsDisplay(\_:)

Marks the specified rectangle of the receiver as needing to be redrawn.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func setNeedsDisplay(_ rect: CGRect)
```

## Parameters 

`rect`  

The rectangular region of the receiver to mark as invalid; it should be specified in the coordinate system of the receiver.

## Discussion

You can use this method or the setNeedsDisplay() to notify the system that your view’s contents need to be redrawn. This method adds the specified rectangle into the view’s current list of invalid rectangles and returns immediately. The view is not actually redrawn until the next drawing cycle, at which point all invalidated views are updated.

Note

If your view is backed by a CAEAGLLayer object, this method has no effect. It is intended for use only with views that use native drawing technologies (such as UIKit and Core Graphics) to render their content.

You should use this method to request that a view be redrawn only when the content or appearance of the view change. If you simply change the geometry of the view, the view is typically not redrawn. Instead, its existing content is adjusted based on the value in the view’s contentMode property. Redisplaying the existing content improves performance by avoiding the need to redraw content that has not changed.

## See Also

### Related Documentation

var contentMode: UIView.ContentMode

A flag used to determine how a view lays out its content when its bounds change.

### Drawing and updating the view

func draw(CGRect)

Draws the view’s image within the passed-in rectangle.

func setNeedsDisplay()

Marks the receiver’s entire bounds rectangle as needing to be redrawn.

var contentScaleFactor: CGFloat

The scale factor applied to the view.

func tintColorDidChange()

Called by the system when the tint color property changes.

