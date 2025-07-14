

- AppKit
- Views and Controls
- NSView
-  Core Animation Support 

API Collection

# Core Animation Support

Manage the layer object that provides the view’s visual representation and accelerates drawing operations.

## Topics

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

var canDrawSubviewsIntoLayer: Bool

A Boolean value indicating whether the view incorporates content from its subviews into its own layer.

var layerUsesCoreImageFilters: Bool

A Boolean value indicating whether the view’s layer uses Core Image filters and needs in-process rendering.

protocol NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

### Managing Layer-Related Properties

var alphaValue: CGFloat

The opacity of the view.

var frameCenterRotation: CGFloat

The rotation angle of the view around the center of its layer.

var backgroundFilters: [CIFilter]

An array of Core Image filters to apply to the view’s background.

var compositingFilter: CIFilter?

The Core Image filter used to composite the view’s contents with its background.

var contentFilters: [CIFilter]

An array of Core Image filters to apply to the contents of the view and its sublayers.

var shadow: NSShadow?

The shadow displayed underneath the view.

## See Also

### Configuring the view

View Hierarchy

Manage the subviews, superview, and window of a view and respond to notifications when the view hierarchy changes.

View Coordinates

Manage the frame and bounds rectangles that determine the size and position of the view in the view hierarchy.

Appearance

Change the view’s visibility, vibrancy, and focus ring and respond to appearance-related changes.

Related UI

Manage contextual menus, cursors, tool tips, and other system-provided windows and content.

