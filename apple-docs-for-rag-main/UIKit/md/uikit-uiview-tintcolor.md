

- UIKit
- UIView
-  tintColor 

Instance Property

# tintColor

The first nondefault tint color value in the view’s hierarchy, ascending from and starting with the view itself.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintColor: UIColor! { get set }
```

## Discussion

If the system cannot find a nondefault color in the hierarchy, this property’s value is a system-defined color instead.

If the view’s tintAdjustmentMode property’s value is UIView.TintAdjustmentMode.dimmed, then the tintColor property value is automatically dimmed.

To refresh subview rendering when this property changes, override the tintColorDidChange() method.

Colors that are pattern colors (as described in UIColor) are not supported.

Important

If you attempt to use a pattern color as a tint color, the system raises an exception.

## See Also

### Related Documentation

func tintColorDidChange()

Called by the system when the tint color property changes.

### Configuring a view’s visual appearance

var backgroundColor: UIColor?

The view’s background color.

var isHidden: Bool

A Boolean value that determines whether the view is hidden.

var alpha: CGFloat

The view’s alpha value.

var isOpaque: Bool

A Boolean value that determines whether the view is opaque.

var tintAdjustmentMode: UIView.TintAdjustmentMode

The first non-default tint adjustment mode value in the view’s hierarchy, ascending from and starting with the view itself.

var clipsToBounds: Bool

A Boolean value that determines whether subviews are confined to the bounds of the view.

var clearsContextBeforeDrawing: Bool

A Boolean value that determines whether the view’s bounds should be automatically cleared before drawing.

var mask: UIView?

An optional view whose alpha channel is used to mask a view’s content.

class var layerClass: AnyClass

Returns the class used to create the layer for instances of this class.

var layer: CALayer

The view’s Core Animation layer to use for rendering.

