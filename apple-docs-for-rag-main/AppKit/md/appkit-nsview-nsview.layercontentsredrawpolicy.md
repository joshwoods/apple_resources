

- AppKit
- NSView
-  NSView.LayerContentsRedrawPolicy 

Enumeration

# NSView.LayerContentsRedrawPolicy

Constants that specify how layer resizing is handled when a view is layer-backed or layer-hosting. For more information, see the layerContentsRedrawPolicy property.

macOS 10.6+

``` source
enum LayerContentsRedrawPolicy
```

## Topics

### Constants

case never

Leave the layer’s contents alone. Never mark the layer as needing display, or draw the view’s contents to the layer. This is how developer created layers (layer-hosting views) are treated.

case onSetNeedsDisplay

Any of the `setNeedsDisplay` methods sent to the view will cause the view redraw the affected layer parts by invoking the view’s draw(_:), but neither the layer or the view are marked as needing display when the view’s size changes.

case duringViewResize

Resize the view’s backing-layer and redraw the view to the layer when the view’s size changes. If the resize is animated, AppKit will drive the resize animation itself and will do this resize and redraw at each step of the animation. Affected parts of the layer will also be redrawn when the view is marked as needing display. This mode is a superset of NSView.LayerContentsRedrawPolicy.onSetNeedsDisplay. This is the way that layer-backed views are currently treated.

case beforeViewResize

Resize the layer and redraw the view to the layer when the view’s size changes. This will be done just once at the beginning of a resize animation, not at each frame of the animation. Affected parts of the layer will also be redrawn when the view is marked as needing display. This mode is a superset of NSView.LayerContentsRedrawPolicy.onSetNeedsDisplay.

case crossfade

Redraw the layer contents at the new size and crossfade from the old contents to the new contents. Use this in conjunction with the NSView.LayerContentsPlacement constants to get a nice crossfade animation for complex layer-backed views that cannot update correctly at each step of the animation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var canDrawSubviewsIntoLayer: Bool

A Boolean value indicating whether the view incorporates content from its subviews into its own layer.

var layerUsesCoreImageFilters: Bool

A Boolean value indicating whether the view’s layer uses Core Image filters and needs in-process rendering.

protocol NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

