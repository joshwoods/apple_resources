

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.oneOverSecondary 

Case

# UISplitViewController.DisplayMode.oneOverSecondary

One sidebar is layered on top of the secondary view controller, leaving the secondary view controller partially visible.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS

``` source
case oneOverSecondary
```

## Discussion

This display mode shows one sidebar layered on top of the secondary view controller, partially obscuring it. The sidebar shown is the primary column for UISplitViewController.Style.doubleColumn interfaces and the supplementary column for UISplitViewController.Style.tripleColumn interfaces. The secondary view controller is dimmed out, preventing interaction with its view. Touching the dimmed view dismisses the overlay and returns the interface to the UISplitViewController.DisplayMode.secondaryOnly display mode.

This display mode is available for the UISplitViewController.SplitBehavior.overlay split behavior.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate display mode based on the device and the current app size.

case secondaryOnly

Only the secondary view controller is shown onscreen.

case oneBesideSecondary

One sidebar appears side-by-side with the secondary view controller.

case twoBesideSecondary

Two sidebars appear side-by-side with the secondary view controller.

case twoOverSecondary

Two sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

