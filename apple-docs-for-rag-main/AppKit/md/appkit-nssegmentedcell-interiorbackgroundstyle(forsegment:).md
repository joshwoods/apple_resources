

- AppKit
- NSSegmentedCell
-  interiorBackgroundStyle(forSegment:) 

Instance Method

# interiorBackgroundStyle(forSegment:)

Returns the interior background style for the specified segment.

macOS 10.5+

``` source
@MainActor
func interiorBackgroundStyle(forSegment segment: Int) -> NSView.BackgroundStyle
```

## Parameters 

`segment`  

The index of the segment whose background style you want to get. This method raises an exception (rangeException) if the index is out of bounds..

## Return Value

The background style to use for specified segment. See NSView.BackgroundStyle for possible values.

## Discussion

The interior background style describes the surface drawn onto in drawInterior(withFrame:in:).

This is both an override point and a useful method to call. In a custom segment cell with a custom bezel, you can override this method to describe the surface on a per-segment basis.

## See Also

### Specifying Segment Visual Styles

var segmentStyle: NSSegmentedControl.Style

The visual style used to display the segmented control.

