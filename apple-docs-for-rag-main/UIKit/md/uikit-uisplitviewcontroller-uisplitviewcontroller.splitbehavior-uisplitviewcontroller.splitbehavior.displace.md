

- UIKit
- UISplitViewController
- UISplitViewController.SplitBehavior
-  UISplitViewController.SplitBehavior.displace 

Case

# UISplitViewController.SplitBehavior.displace

The sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
case displace
```

## Discussion

This split behavior shows one or both sidebars tiled next to the secondary view controller. If both sidebars are visible, they partially displace the secondary view controller offscreen to make space for the primary column. The secondary view controller is dimmed out, preventing interaction with its view.

The possible display modes for this split behavior are:

- UISplitViewController.DisplayMode.secondaryOnly

- UISplitViewController.DisplayMode.oneBesideSecondary

- UISplitViewController.DisplayMode.twoDisplaceSecondary

If the current display mode is UISplitViewController.DisplayMode.oneBesideSecondary and presentsWithGesture is true, the split view controller presents a special bar button item styled as a back-chevron icon. When a user taps this button, it changes the current display mode to UISplitViewController.DisplayMode.twoDisplaceSecondary.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate split behavior based on the device and the current app size.

case tile

The sidebars and secondary view controller appear tiled side-by-side.

case overlay

The sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

