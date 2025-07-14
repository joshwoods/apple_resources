

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.twoDisplaceSecondary 

Case

# UISplitViewController.DisplayMode.twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
case twoDisplaceSecondary
```

## Discussion

This display mode is only available for UISplitViewController.Style.tripleColumn interfaces.

This display mode shows both sidebars, which partially displace the secondary view controller offscreen to make space for the primary column. The secondary view controller is dimmed out, preventing interaction with its view. Touching the dimmed view or using a gesture returns the interface to the UISplitViewController.DisplayMode.oneBesideSecondary display mode.

This display mode is available for the UISplitViewController.SplitBehavior.displace split behavior.

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

case twoOverSecondary

Two sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

