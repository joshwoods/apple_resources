

- AppKit
-  NSViewLayerContentScaleDelegate 

Protocol

# NSViewLayerContentScaleDelegate

An optional layer delegate method for handling resolution changes.

macOS

``` source
protocol NSViewLayerContentScaleDelegate : NSObjectProtocol
```

## Overview

Use this protocol to manage scale and contents for a layer hosted in a view. When a window changes its backing resolution, AppKit attempts to automatically update the `contentsScale` and `contents` of all `CALayer` objects in the window to match the new resolution. Layers backed by a view are updated automatically. Any layer whose `contents` property is set to an `NSImage` object is also updated automatically. Based on the `NSImage` object’s available representations, AppKit selects an appropriate bitmapped representation, or rasterizes a resolution-independent representation at the appropriate scale factor.

For all other layers, AppKit checks whether the layer has a delegate that implements this protocol. If so, AppKit asks the layer’s delegate whether it should automatically update the `contentsScale` for that layer to match the new scale factor of the window.

## Topics

### Responding to Resolution Changes

func layer(CALayer, shouldInheritContentsScale: CGFloat, from: NSWindow) -> Bool

Notifies you when a resolution changes occurs for the window that hosts the layer.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

View Programming Guide

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

