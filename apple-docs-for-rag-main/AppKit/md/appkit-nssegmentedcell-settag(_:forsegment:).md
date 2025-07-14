

- AppKit
- NSSegmentedCell
-  setTag(\_:forSegment:) 

Instance Method

# setTag(\_:forSegment:)

Sets the tag for the specified segment.

macOS

``` source
@MainActor
func setTag(
    _ tag: Int,
    forSegment segment: Int
)
```

## Parameters 

`tag`  

The tag of the segment.

`segment`  

The index of the segment whose tool tag you want to set. This method raises an exception (rangeException) if the index is out of bounds.

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

func isEnabled(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is enabled.

func setMenu(NSMenu?, forSegment: Int)

Sets the menu for the specified segment.

func menu(forSegment: Int) -> NSMenu?

Returns the menu for the specified segment.

func setToolTip(String?, forSegment: Int)

Sets the tooltip for the specified segment.

func toolTip(forSegment: Int) -> String?

Returns the tooltip of the specified segment.

func tag(forSegment: Int) -> Int

Returns the tag of the specified segment.

