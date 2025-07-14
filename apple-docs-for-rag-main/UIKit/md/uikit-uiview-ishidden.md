

- UIKit
- UIView
-  isHidden 

Instance Property

# isHidden

A Boolean value that determines whether the view is hidden.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isHidden: Bool { get set }
```

## Discussion

Setting the value of this property to true hides the receiver and setting it to false shows the receiver. The default value is false.

A hidden view disappears from its window and does not receive input events. It remains in its superview’s list of subviews, however, and participates in autoresizing as usual. Hiding a view with subviews has the effect of hiding those subviews and any view descendants they might have. This effect is implicit and does not alter the hidden state of the receiver’s descendants.

Hiding the view that is the window’s current first responder causes the view’s next valid key view to become the new first responder.

The value of this property reflects the state of the receiver only and does not account for the state of the receiver’s ancestors in the view hierarchy. Thus this property can be false but the receiver may still be hidden if an ancestor is hidden.

## See Also

### Configuring a view’s visual appearance

var backgroundColor: UIColor?

The view’s background color.

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

var layer: CALayer

The view’s Core Animation layer to use for rendering.

