

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.oneBesideSecondary 

Case

# UISplitViewController.DisplayMode.oneBesideSecondary

One sidebar appears side-by-side with the secondary view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case oneBesideSecondary
```

## Discussion

This display mode shows one sidebar tiled next to the secondary view controller. The sidebar shown is the primary column for UISplitViewController.Style.doubleColumn interfaces and the supplementary column for UISplitViewController.Style.tripleColumn interfaces. The sidebar is displayed on the side specified by primaryEdge, followed by the secondary view controller. The secondary view controller’s view is fully interactive.

This display mode is available for the UISplitViewController.SplitBehavior.tile and UISplitViewController.SplitBehavior.displace split behaviors.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate display mode based on the device and the current app size.

case secondaryOnly

Only the secondary view controller is shown onscreen.

case oneOverSecondary

One sidebar is layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case twoBesideSecondary

Two sidebars appear side-by-side with the secondary view controller.

case twoOverSecondary

Two sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

