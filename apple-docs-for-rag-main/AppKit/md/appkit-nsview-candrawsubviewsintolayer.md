

- AppKit
- NSView
-  canDrawSubviewsIntoLayer 

Instance Property

# canDrawSubviewsIntoLayer

A Boolean value indicating whether the view incorporates content from its subviews into its own layer.

macOS 10.9+

``` source
@MainActor
var canDrawSubviewsIntoLayer: Bool { get set }
```

## Discussion

When the value of this property is true, any subviews that have an implicitly created layer—that is, layers for which you did not explicitly set the wantsLayer property to true—draw their contents into the current view’s layer. In other words, the subviews do not get a layer of their own. Instead, they draw their content into the parent view’s layer. All views involved in the operation draw their content using their draw(_:) method. They do not use the updateLayer() method to update their layer contents, even if the wantsUpdateLayer property is set to true.

Use this property to flatten the layer hierarchy for a layer-backed view and its subviews. Flattening a layer hierarchy reduces the number of layers (and may reduce the amount of memory) used by your view hierarchy. Reducing the number of layers can be more efficient in situations where there is significant overlap among the subviews or where the content of the view and subviews does not change significantly. For example, flattening a hierarchy reduces the amount of time spent compositing your views together. Do not flatten a view hierarchy if you plan to animate one or more subviews in that hierarchy.

When changing the value of this property, the current view must have a layer object. The default value of this property is false.

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

var layerContentsRedrawPolicy: NSView.LayerContentsRedrawPolicy

The contents redraw policy for the view’s layer.

enum LayerContentsRedrawPolicy

Constants that specify how layer resizing is handled when a view is layer-backed or layer-hosting. For more information, see the layerContentsRedrawPolicy property.

var layerUsesCoreImageFilters: Bool

A Boolean value indicating whether the view’s layer uses Core Image filters and needs in-process rendering.

protocol NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

