

- AppKit
- NSSegmentedControl
-  menu(forSegment:) 

Instance Method

# menu(forSegment:)

Returns the menu for the specified segment.

macOS

``` source
@MainActor
func menu(forSegment segment: Int) -> NSMenu?
```

## Parameters 

`segment`  

The index of the segment whose menu you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

The menu associated with the segment; otherwise, `nil`.

## See Also

### Configuring a Segment Menu

func setMenu(NSMenu?, forSegment: Int)

Sets the menu for the specified segment.

func setShowsMenuIndicator(Bool, forSegment: Int)

func showsMenuIndicator(forSegment: Int) -> Bool

var isSpringLoaded: Bool

A Boolean value that indicates whether spring loading is enabled for the control.

