

- AppKit
- NSView
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a size from the view’s coordinate system to that of another view.

macOS

``` source
@MainActor
func convert(
    _ size: NSSize,
    to view: NSView?
) -> NSSize
```

## Parameters 

`size`  

The size (width and height) in the view’s coordinate system.

`view`  

The view that’s the target of the conversion operation. Both `view` and the view must belong to the same NSWindow object, and that window must not be `nil`. If `view` is `nil`, this method converts to window coordinates instead.

## Return Value

The converted size, as an NSSize structure.

## Discussion

The returned `NSSize` values are always forced to have positive a width and height.

## See Also

### Related Documentation

var contentView: NSView?

The window’s content view, the highest accessible view object in the window’s view hierarchy.

func ancestorShared(with: NSView) -> NSView?

Returns the closest ancestor shared by the view and another specified view.

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

func convertToLayer(NSSize) -> NSSize

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

