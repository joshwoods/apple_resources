

- UIKit
- UIView
-  mask 

Instance Property

# mask

An optional view whose alpha channel is used to mask a view’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var mask: UIView? { get set }
```

## Discussion

The view’s alpha channel determines how much of the view’s content and background shows through. Fully or partially opaque pixels allow the underlying content to show through but fully transparent pixels block that content.

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

var clearsContextBeforeDrawing: Bool

A Boolean value that determines whether the view’s bounds should be automatically cleared before drawing.

class var layerClass: AnyClass

Returns the class used to create the layer for instances of this class.

var layer: CALayer

The view’s Core Animation layer to use for rendering.

