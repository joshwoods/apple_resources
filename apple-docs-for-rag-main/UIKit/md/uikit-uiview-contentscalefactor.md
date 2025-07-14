

- UIKit
- UIView
-  contentScaleFactor 

Instance Property

# contentScaleFactor

The scale factor applied to the view.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentScaleFactor: CGFloat { get set }
```

## Discussion

The scale factor determines how content in the view is mapped from the logical coordinate space (measured in points) to the device coordinate space (measured in pixels). This value is typically either `1.0` or `2.0`. Higher scale factors indicate that each point in the view is represented by more than one pixel in the underlying layer. For example, if the scale factor is `2.0` and the view frame size is 50 x 50 points, the size of the bitmap used to present that content is 100 x 100 pixels.

The default value for this property is the scale factor associated with the screen currently displaying the view. If your custom view implements a custom draw(_:) method and is associated with a window, or if you use the GLKView class to draw OpenGL ES content, your view draws at the full resolution of the screen. For system views, the value of this property may be `1.0` even on high resolution screens.

In general, you should not need to modify the value in this property. However, if your application draws using OpenGL ES, you may want to change the scale factor to trade image quality for rendering performance. For more information on how to adjust your OpenGL ES rendering environment, see Supporting High-Resolution Displays in OpenGL ES Programming Guide.

## See Also

### Drawing and updating the view

func draw(CGRect)

Draws the view’s image within the passed-in rectangle.

func setNeedsDisplay()

Marks the receiver’s entire bounds rectangle as needing to be redrawn.

func setNeedsDisplay(CGRect)

Marks the specified rectangle of the receiver as needing to be redrawn.

func tintColorDidChange()

Called by the system when the tint color property changes.

