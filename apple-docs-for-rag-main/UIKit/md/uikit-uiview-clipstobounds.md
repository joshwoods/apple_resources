

- UIKit
- UIView
-  clipsToBounds 

Instance Property

# clipsToBounds

A Boolean value that determines whether subviews are confined to the bounds of the view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var clipsToBounds: Bool { get set }
```

## Mentioned in 

Using responders and the responder chain to handle events

## Discussion

Setting this value to true causes subviews to be clipped to the bounds of the view. If set to false, subviews whose frames extend beyond the visible bounds of the view aren’t clipped.

The default value is false. Some subclasses of UIView, like UIScrollView, override the default value to true.

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

var clearsContextBeforeDrawing: Bool

A Boolean value that determines whether the view’s bounds should be automatically cleared before drawing.

var mask: UIView?

An optional view whose alpha channel is used to mask a view’s content.

class var layerClass: AnyClass

Returns the class used to create the layer for instances of this class.

var layer: CALayer

The view’s Core Animation layer to use for rendering.

