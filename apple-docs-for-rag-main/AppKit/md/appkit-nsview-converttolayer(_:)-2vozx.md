

- AppKit
- NSView
-  convertToLayer(\_:) 

Instance Method

# convertToLayer(\_:)

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

macOS 10.7+

``` source
@MainActor
func convertToLayer(_ size: NSSize) -> NSSize
```

## Parameters 

`size`  

A size in the view’s interior coordinate system.

## Return Value

A size in the layer’s interior coordinate system.

## Discussion

The layer’s space is virtual, and doesn’t take into account the layer’s contentsScale setting.

The returned `NSSize` values are always forced to have positive a width and height.

## See Also

### Converting Coordinate Values

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Returns a backing store pixel-aligned rectangle in local view coordinates.

func convertFromBacking(NSPoint) -> NSPoint

Converts a point from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSPoint) -> NSPoint

Converts a point from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSPoint) -> NSPoint

Convert the point from the layer’s interior coordinate system to the view’s interior coordinate system.

func convertToLayer(NSPoint) -> NSPoint

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convertFromBacking(NSRect) -> NSRect

Converts a rectangle from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSRect) -> NSRect

Converts a rectangle from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSRect) -> NSRect

Convert the rectangle from the layer’s interior coordinate system to the view’s interior coordinate system.

func convertToLayer(NSRect) -> NSRect

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convertFromBacking(NSSize) -> NSSize

Converts a size from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSSize) -> NSSize

Converts a size from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSSize) -> NSSize

Convert the size from the layer’s interior coordinate system to the view’s interior coordinate system.

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

func convert(NSSize, from: NSView?) -> NSSize

Converts a size from another view’s coordinate system to that of the view.

