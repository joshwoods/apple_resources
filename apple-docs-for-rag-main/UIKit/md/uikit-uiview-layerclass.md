

- UIKit
- UIView
-  layerClass 

Type Property

# layerClass

Returns the class used to create the layer for instances of this class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var layerClass: AnyClass { get }
```

## Return Value

The class used to create the view’s Core Animation layer.

## Discussion

This method returns the CALayer class object by default. Subclasses can override this method and return a different layer class as needed. For example, if your view uses tiling to display a large scrollable area, you might want to override this property and return the CATiledLayer class, as shown in the following code.

```
override class var layerClass : AnyClass {
   return CATiledLayer.self
}
```

This method is called only once early in the creation of the view in order to create the corresponding layer object.

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

var layer: CALayer

The view’s Core Animation layer to use for rendering.

