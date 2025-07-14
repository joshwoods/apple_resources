

- UIKit
- UISplitViewController
- UISplitViewController.SplitBehavior
-  UISplitViewController.SplitBehavior.tile 

Case

# UISplitViewController.SplitBehavior.tile

The sidebars and secondary view controller appear tiled side-by-side.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
case tile
```

## Discussion

This split behavior shows one or both sidebars tiled next to the secondary view controller. The secondary view controller’s view is fully interactive.

The possible display modes for this split behavior are:

- UISplitViewController.DisplayMode.secondaryOnly

- UISplitViewController.DisplayMode.oneBesideSecondary

- UISplitViewController.DisplayMode.twoBesideSecondary

If presentsWithGesture is true, the split view controller presents a special bar button item styled as a sidebar toggle icon.

For a double-column split view interface, when a user taps this button, it toggles the current display mode between UISplitViewController.DisplayMode.secondaryOnly and UISplitViewController.DisplayMode.oneBesideSecondary.

For a triple-column split view interface, when a user taps this button, it toggles the current display mode between UISplitViewController.DisplayMode.oneBesideSecondary and UISplitViewController.DisplayMode.twoBesideSecondary. The button doesn’t appear in UISplitViewController.DisplayMode.secondaryOnly.

## See Also

### Constants

case automatic

The split view controller automatically decides the most appropriate split behavior based on the device and the current app size.

case overlay

The sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case displace

The sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

