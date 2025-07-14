

- UIKit
- UISplitViewController
- UISplitViewController.DisplayMode
-  UISplitViewController.DisplayMode.automatic 

Case

# UISplitViewController.DisplayMode.automatic

The split view controller automatically decides the most appropriate display mode based on the device and the current app size.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case automatic
```

## Discussion

This constant represents the default value of the preferredDisplayMode property. Although you can assign the property this constant as its value, the displayMode property never reports it.

## See Also

### Constants

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

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

