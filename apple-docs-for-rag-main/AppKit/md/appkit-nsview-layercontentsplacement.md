

- AppKit
- NSView
-  layerContentsPlacement 

Instance Property

# layerContentsPlacement

The current layer contents placement policy.

macOS 10.6+

``` source
@MainActor
var layerContentsPlacement: NSView.LayerContentsPlacement { get set }
```

## Discussion

The content placement determines how the backing layer’s existing cached content image will be mapped into the layer as the layer is resized. It is analogous to, and underpinned by, the contentsGravity property of the CALayer class. The default value of this property is NSView.LayerContentsPlacement.scaleAxesIndependently. For a list of supported values, see NSView.LayerContentsPlacement.

For additional information about the performance impacts of this property, see the layerContentsRedrawPolicy property.

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

