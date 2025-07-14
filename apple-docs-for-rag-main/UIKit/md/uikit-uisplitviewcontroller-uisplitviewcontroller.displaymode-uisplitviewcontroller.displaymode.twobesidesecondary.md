

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.twoBesideSecondary 

Case

# UISplitViewController.DisplayMode.twoBesideSecondary

Two sidebars appear side-by-side with the secondary view controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
case twoBesideSecondary
```

## Discussion

This display mode is only available for UISplitViewController.Style.tripleColumn interfaces.

This display mode shows both sidebars tiled next to the secondary view controller. The primary view controller is displayed on the side specified by primaryEdge, followed by the supplementary view controller, and finally the secondary view controller. The secondary view controller’s view is fully interactive.

This display mode is available for the UISplitViewController.SplitBehavior.tile split behavior.

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

case twoOverSecondary

Two sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

