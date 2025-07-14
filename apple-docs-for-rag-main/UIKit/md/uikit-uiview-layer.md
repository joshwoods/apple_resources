

- UIKit
- UIView
-  layer 

Instance Property

# layer

The view’s Core Animation layer to use for rendering.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var layer: CALayer { get }
```

## Discussion

This property is never `nil`. The value of the layerClass property determines the actual class of the layer object. The view is the layer’s delegate.

Warning

Because the view is the layer’s delegate, never make the view the delegate of another CALayer object. Additionally, never change the delegate of this layer object.

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

var mask: UIView?

An optional view whose alpha channel is used to mask a view’s content.

class var layerClass: AnyClass

Returns the class used to create the layer for instances of this class.

