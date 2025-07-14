

- AppKit
- NSView
-  backingAlignedRect(\_:options:) 

Instance Method

# backingAlignedRect(\_:options:)

Returns a backing store pixel-aligned rectangle in local view coordinates.

macOS 10.7+

``` source
@MainActor
func backingAlignedRect(
    _ rect: NSRect,
    options: AlignmentOptions = []
) -> NSRect
```

## Parameters 

`rect`  

The rectangle in the view’s interior coordinate system.

`options`  

The alignment options. See AlignmentOptions for possible values. (Note that although the alignment options specify integral values, the rectangle returned by this method is pixel-aligned.)

## Return Value

A rectangle in the view’s interior coordinate system that is aligned to the backing store pixels using the specified options.

## Discussion

Uses the NSIntegralRectWithOptions(_:_:) function and the given input rectangle and options to produce a backing store pixel-aligned rectangle in the view’s interior coordinates.

## See Also

### Converting Coordinate Values

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

func convertToLayer(NSSize) -> NSSize

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

func convert(NSSize, from: NSView?) -> NSSize

Converts a size from another view’s coordinate system to that of the view.

