

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.twoOverSecondary 

Case

# UISplitViewController.DisplayMode.twoOverSecondary

Two sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
case twoOverSecondary
```

## Discussion

This display mode is only available for UISplitViewController.Style.tripleColumn interfaces.

This display mode shows both sidebars layered on top of the secondary view controller, partially obscuring it. The secondary view controller is dimmed out, preventing interaction with its view. Touching the dimmed view dismisses the overlay and returns the interface to the UISplitViewController.DisplayMode.secondaryOnly display mode.

The interactive gesture can move the interface freely through UISplitViewController.DisplayMode.oneOverSecondary to UISplitViewController.DisplayMode.secondaryOnly and back, stopping at any of the display modes depending on the user interaction.

This display mode is available for the UISplitViewController.SplitBehavior.overlay split behavior.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate display mode based on the device and the current app size.

case secondaryOnly

Only the secondary view controller is shown onscreen.

case oneBesideSecondary

One sidebar appears side-by-side with the secondary view controller.

case oneOverSecondary

One sidebar is layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case twoBesideSecondary

Two sidebars appear side-by-side with the secondary view controller.

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

