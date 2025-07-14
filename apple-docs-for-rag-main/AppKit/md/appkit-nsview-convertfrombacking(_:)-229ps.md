

- AppKit
- NSView
-  convertFromBacking(\_:) 

Instance Method

# convertFromBacking(\_:)

Converts a point from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

macOS 10.7+

``` source
@MainActor
func convertFromBacking(_ point: NSPoint) -> NSPoint
```

## Parameters 

`point`  

The point in the pixel backing store aligned coordinate system.

## Return Value

A point in the view’s interior coordinate system.

## See Also

### Converting Coordinate Values

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Returns a backing store pixel-aligned rectangle in local view coordinates.

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

func convertToLayer(NSSize) -> NSSize

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

func convert(NSSize, from: NSView?) -> NSSize

Converts a size from another view’s coordinate system to that of the view.

