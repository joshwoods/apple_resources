

- AppKit
- NSSegmentedControl
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

The menu you want to add to the segment or `nil` to clear the current menu.

`segment`  

The index of the segment whose menu you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## Discussion

Adding a menu to a segment allows the segment to be used as a pop-up button. If the segment has a menu only, then the menu displays when the user clicks the segment. If the segment has both a menu and an action, then the action triggers when the user clicks the segment and the menu displays when the user clicks and holds the segment.

## See Also

### Configuring a Segment Menu

func menu(forSegment: Int) -> NSMenu?

Returns the menu for the specified segment.

func setShowsMenuIndicator(Bool, forSegment: Int)

func showsMenuIndicator(forSegment: Int) -> Bool

var isSpringLoaded: Bool

A Boolean value that indicates whether spring loading is enabled for the control.

