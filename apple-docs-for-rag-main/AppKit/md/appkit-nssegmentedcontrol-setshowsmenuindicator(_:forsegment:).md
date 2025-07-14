

- AppKit
- NSSegmentedControl
-  setShowsMenuIndicator(\_:forSegment:) 

Instance Method

# setShowsMenuIndicator(\_:forSegment:)

macOS 10.13+

``` source
@MainActor
func setShowsMenuIndicator(
    _ showsMenuIndicator: Bool,
    forSegment segment: Int
)
```

## See Also

### Configuring a Segment Menu

func setMenu(NSMenu?, forSegment: Int)

Sets the menu for the specified segment.

func menu(forSegment: Int) -> NSMenu?

Returns the menu for the specified segment.

func showsMenuIndicator(forSegment: Int) -> Bool

var isSpringLoaded: Bool

A Boolean value that indicates whether spring loading is enabled for the control.

