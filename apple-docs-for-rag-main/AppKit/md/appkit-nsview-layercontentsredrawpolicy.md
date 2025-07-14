

- AppKit
- NSView
-  layerContentsRedrawPolicy 

Instance Property

# layerContentsRedrawPolicy

The contents redraw policy for the view’s layer.

macOS 10.6+

``` source
@MainActor
var layerContentsRedrawPolicy: NSView.LayerContentsRedrawPolicy { get set }
```

## Discussion

The layerContentsRedrawPolicy and layerContentsPlacement settings can have significant impacts on performance. If you do not need to redraw your view during each frame update cycle, or if you are willing to accept an approximation of the view’s intermediate appearance during potentially brief animations in exchange for an animation performance and smoothness benefit, you can change the value of this property to one of the modes that does not require constant redrawing. When you do so, you must also specify the desired layer content placement for the view. The content placement determines how the backing layer’s existing cached content image will be mapped into the layer as the layer is resized. It is analogous to, and underpinned by, the contentsGravity property of the CALayer class.

For a view that has no associated layer, or that has been assigned a developer-provided layer (a layer-hosting view) using the layer property, the default contents redraw policy is NSView.LayerContentsRedrawPolicy.never and the layerContentsPlacement property is set to NSView.LayerContentsPlacement.scaleAxesIndependently. These policies tell AppKit not to replace the layer’s content and to provide the same content placement as the resize option.For a layer-backed view—that is, a view for which AppKit created the layer—AppKit sets the contents redraw policy to NSView.LayerContentsRedrawPolicy.duringViewResize by default. This policy forces the view’s content to be continually redrawn into the view’s backing layer during animated resizing of the view, which produces correct but not optimal performance results.

## See Also

### Managing the View’s Layer

var wantsLayer: Bool

A Boolean value indicating whether the view uses a layer as its backing store.

var wantsUpdateLayer: Bool

A Boolean value indicating which drawing path the view takes when updating its contents.

var layer: CALayer?

The Core Animation layer that the view uses as its backing store.

func makeBackingLayer() -> CALayer

Creates the view’s backing layer.

var layerContentsPlacement: NSView.LayerContentsPlacement

The current layer contents placement policy.

enum LayerContentsPlacement

These constants specify the location of the layer content when the content is not rerendered in response to view resizing. For more information, see the layerContentsPlacement property.

enum LayerContentsRedrawPolicy

Constants that specify how layer resizing is handled when a view is layer-backed or layer-hosting. For more information, see the layerContentsRedrawPolicy property.

var canDrawSubviewsIntoLayer: Bool

A Boolean value indicating whether the view incorporates content from its subviews into its own layer.

var layerUsesCoreImageFilters: Bool

A Boolean value indicating whether the view’s layer uses Core Image filters and needs in-process rendering.

protocol NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

