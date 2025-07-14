

- UIKit
- UIView
-  clearsContextBeforeDrawing 

Instance Property

# clearsContextBeforeDrawing

A Boolean value that determines whether the view’s bounds should be automatically cleared before drawing.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var clearsContextBeforeDrawing: Bool { get set }
```

## Discussion

When set to true, the drawing buffer is automatically cleared to transparent black before the draw(_:) method is called. This behavior ensures that there are no visual artifacts left over when the view’s contents are redrawn. If the view’s isOpaque property is also set to true, the backgroundColor property of the view must not be `nil` or drawing errors may occur. The default value of this property is true.

If you set the value of this property to false, you are responsible for ensuring the contents of the view are drawn properly in your draw(_:) method. If your drawing code is already heavily optimized, setting this property is false can improve performance, especially during scrolling when only a portion of the view might need to be redrawn.

## See Also

### Configuring a view’s visual appearance

var backgroundColor: UIColor?

The view’s background color.

var isHidden: Bool

A Boolean value that determines whether the view is hidden.

var alpha: CGFloat

The view’s alpha value.

var isOpaque: Bool

A Boolean value that determines whether the view is opaque.

var tintColor: UIColor!

The first nondefault tint color value in the view’s hierarchy, ascending from and starting with the view itself.

var tintAdjustmentMode: UIView.TintAdjustmentMode

The first non-default tint adjustment mode value in the view’s hierarchy, ascending from and starting with the view itself.

var clipsToBounds: Bool

A Boolean value that determines whether subviews are confined to the bounds of the view.

var mask: UIView?

An optional view whose alpha channel is used to mask a view’s content.

class var layerClass: AnyClass

Returns the class used to create the layer for instances of this class.

var layer: CALayer

The view’s Core Animation layer to use for rendering.

