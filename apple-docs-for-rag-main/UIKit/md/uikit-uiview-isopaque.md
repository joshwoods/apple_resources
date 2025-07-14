

- UIKit
- UIView
-  isOpaque 

Instance Property

# isOpaque

A Boolean value that determines whether the view is opaque.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isOpaque: Bool { get set }
```

## Discussion

This property provides a hint to the drawing system as to how it should treat the view. If set to true, the drawing system treats the view as fully opaque, which allows the drawing system to optimize some drawing operations and improve performance. If set to false, the drawing system composites the view normally with other content. The default value of this property is true.

An opaque view is expected to fill its bounds with entirely opaque content—that is, the content should have an alpha value of `1.0`. If the view is opaque and either does not fill its bounds or contains wholly or partially transparent content, the results are unpredictable. You should always set the value of this property to false if the view is fully or partially transparent.

You only need to set a value for the opaque property in subclasses of UIView that draw their own content using the draw(_:) method. The opaque property has no effect in system-provided classes such as UIButton, UILabel, UITableViewCell, and so on.

## See Also

### Configuring a view’s visual appearance

var backgroundColor: UIColor?

The view’s background color.

var isHidden: Bool

A Boolean value that determines whether the view is hidden.

var alpha: CGFloat

The view’s alpha value.

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

