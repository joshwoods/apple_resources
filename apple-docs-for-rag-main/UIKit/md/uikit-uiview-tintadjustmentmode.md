

- UIKit
- UIView
-  tintAdjustmentMode 

Instance Property

# tintAdjustmentMode

The first non-default tint adjustment mode value in the view’s hierarchy, ascending from and starting with the view itself.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintAdjustmentMode: UIView.TintAdjustmentMode { get set }
```

## Discussion

When this property’s value is UIView.TintAdjustmentMode.dimmed, the value of the tintColor property is modified to provide a dimmed appearance.

If the system cannot find a non-default value in the subview hierarchy when you query this property, the value is UIView.TintAdjustmentMode.normal.

When this property’s value changes (either by the view’s value changing or by one of its superview’s values changing), the system calls the tintColorDidChange() method to allow the view to refresh its rendering.

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

