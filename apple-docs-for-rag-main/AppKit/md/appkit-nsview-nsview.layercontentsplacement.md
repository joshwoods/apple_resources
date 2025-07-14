

- AppKit
- NSView
-  NSView.LayerContentsPlacement 

Enumeration

# NSView.LayerContentsPlacement

These constants specify the location of the layer content when the content is not rerendered in response to view resizing. For more information, see the layerContentsPlacement property.

macOS 10.6+

``` source
enum LayerContentsPlacement
```

## Topics

### Constants

case scaleAxesIndependently

The content is resized to fit the entire bounds rectangle.

case scaleProportionallyToFit

The content is resized to fit the bounds rectangle, preserving the aspect of the content. If the content does not completely fill the bounds rectangle, the content is centered in the partial axis.

case scaleProportionallyToFill

The content is resized to completely fill the bounds rectangle, while still preserving the aspect of the content. The content is centered in the axis it exceeds.

case center

The content is horizontally and vertically centered in the bounds rectangle.

case top

The content is horizontally centered at the top-edge of the bounds rectangle.

case topRight

The content is positioned in the top-right corner of the bounds rectangle.

case right

The content is vertically centered at the right-edge of the bounds rectangle.

case bottomRight

The content is positioned in the bottom-right corner of the bounds rectangle.

case bottom

The content is horizontally centered at the bottom-edge of the bounds rectangle.

case bottomLeft

The content is positioned in the bottom-left corner of the bounds rectangle.

case left

The content is vertically centered at the left-edge of the bounds rectangle.

case topLeft

The content is positioned in the top-left corner of the bounds rectangle.

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

