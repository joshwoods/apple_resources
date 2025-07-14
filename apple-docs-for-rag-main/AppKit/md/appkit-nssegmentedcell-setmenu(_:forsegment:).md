

- AppKit
- NSSegmentedCell
-  setMenu(\_:forSegment:) 

Instance Method

# setMenu(\_:forSegment:)

Sets the menu for the specified segment.

macOS

``` source
@MainActor
func setMenu(
    _ menu: NSMenu?,
    forSegment segment: Int
)
```

## Parameters 

`menu`  

The menu you want to add to the segment or `nil` to clear the current menu. This menu is displayed when the user clicks and holds the mouse button while the mouse is over the segment.

`segment`  

The index of the segment whose menu you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## Discussion

Adding a menu to a segment allows that segment to be used as a pop-up button.

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

