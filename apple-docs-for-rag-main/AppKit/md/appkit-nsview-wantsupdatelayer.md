

- AppKit
- NSView
-  wantsUpdateLayer 

Instance Property

# wantsUpdateLayer

A Boolean value indicating which drawing path the view takes when updating its contents.

macOS 10.8+

``` source
@MainActor
var wantsUpdateLayer: Bool { get }
```

## Discussion

A view can update its contents using one of two techniques. It can draw those contents using its draw(_:) method or it can modify its underlying layer object directly. During the view update cycle, each dirty view calls this method on itself to determine which technique to use. The default implementation of this method returns false, which causes the view to use its draw(_:) method.

If your view is layer-backed and updates itself by modifying its layer, override this property and change the return value to true. Modifying the layer is significantly faster than redrawing the layer contents using draw(_:). If you override this property to be true, you must also override the updateLayer() method of your view and use it to make the changes to your layer. Do not modify your layer in your implementation of this property. Your implementation should return true or false quickly and not perform other tasks.

If the canDrawSubviewsIntoLayer property is set to true, the view ignores the value returned by this method. Instead, the view always uses its draw(_:) method to draw its content.

Note

When using the updateLayer() method to update your view, it is recommended that you set the view’s redraw policy to NSView.LayerContentsRedrawPolicy.onSetNeedsDisplay. This policy lets you control when you want to update the layer’s contents.

## See Also

### Related Documentation

func updateLayer()

Updates the view’s content by modifying its underlying layer.

### Managing the View’s Layer

var wantsLayer: Bool

A Boolean value indicating whether the view uses a layer as its backing store.

var layer: CALayer?

The Core Animation layer that the view uses as its backing store.

func makeBackingLayer() -> CALayer

Creates the view’s backing layer.

var layerContentsPlacement: NSView.LayerContentsPlacement

The current layer contents placement policy.

enum LayerContentsPlacement

These constants specify the location of the layer content when the content is not rerendered in response to view resizing. For more information, see the layerContentsPlacement property.

var layerContentsRedrawPolicy: NSView.LayerContentsRedrawPolicy

The contents redraw policy for the view’s layer.

enum LayerContentsRedrawPolicy

Constants that specify how layer resizing is handled when a view is layer-backed or layer-hosting. For more information, see the layerContentsRedrawPolicy property.

var canDrawSubviewsIntoLayer: Bool

A Boolean value indicating whether the view incorporates content from its subviews into its own layer.

var layerUsesCoreImageFilters: Bool

A Boolean value indicating whether the view’s layer uses Core Image filters and needs in-process rendering.

protocol NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

