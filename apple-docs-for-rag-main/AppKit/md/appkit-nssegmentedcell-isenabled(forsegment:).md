

- AppKit
- NSSegmentedCell
-  isEnabled(forSegment:) 

Instance Method

# isEnabled(forSegment:)

Returns a Boolean value indicating whether the specified segment is enabled.

macOS

``` source
@MainActor
func isEnabled(forSegment segment: Int) -> Bool
```

## Parameters 

`segment`  

The index of the segment whose enabled state you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

true if the segment is enabled; otherwise, false.

## See Also

### Configuring Individual Segments

func setLabel(String, forSegment: Int)

Sets the label for the specified segment.

func label(forSegment: Int) -> String?

Returns the label of the specified segment.

func setImage(NSImage?, forSegment: Int)

Sets the image for the specified segment.

func image(forSegment: Int) -> NSImage?

Returns the image associated with the specified segment.

func setImageScaling(NSImageScaling, forSegment: Int)

Sets the image scaling mode for the specified segment.

func imageScaling(forSegment: Int) -> NSImageScaling

Returns the image scaling mode associated with the specified segment.

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

func setEnabled(Bool, forSegment: Int)

Sets the enabled state of the specified segment

func setMenu(NSMenu?, forSegment: Int)

Sets the menu for the specified segment.

func menu(forSegment: Int) -> NSMenu?

Returns the menu for the specified segment.

func setToolTip(String?, forSegment: Int)

Sets the tooltip for the specified segment.

func toolTip(forSegment: Int) -> String?

Returns the tooltip of the specified segment.

func setTag(Int, forSegment: Int)

Sets the tag for the specified segment.

func tag(forSegment: Int) -> Int

Returns the tag of the specified segment.

