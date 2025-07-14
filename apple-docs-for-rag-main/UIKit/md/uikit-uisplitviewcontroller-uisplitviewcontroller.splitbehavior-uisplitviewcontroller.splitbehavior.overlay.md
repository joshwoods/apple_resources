

- UIKit
- UISplitViewController
- UISplitViewController.SplitBehavior
-  UISplitViewController.SplitBehavior.overlay 

Case

# UISplitViewController.SplitBehavior.overlay

The sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
case overlay
```

## Discussion

This split behavior shows one or both sidebars layered on top of the secondary view controller, partially obscuring it. The secondary view controller is dimmed out, preventing interaction with its view.

The possible display modes for this split behavior are:

- UISplitViewController.DisplayMode.secondaryOnly

- UISplitViewController.DisplayMode.oneOverSecondary

- UISplitViewController.DisplayMode.twoOverSecondary

If the current display mode is not UISplitViewController.DisplayMode.twoOverSecondary and presentsWithGesture is true, the split view controller presents a special bar button item styled as a back-chevron icon. When a user taps this button, it changes the current display mode from UISplitViewController.DisplayMode.secondaryOnly to UISplitViewController.DisplayMode.oneOverSecondary, and from UISplitViewController.DisplayMode.oneOverSecondary to UISplitViewController.DisplayMode.twoOverSecondary.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate split behavior based on the device and the current app size.

case tile

The sidebars and secondary view controller appear tiled side-by-side.

case displace

The sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

