

- UIKit
- UISplitViewController
-  UISplitViewController.SplitBehavior 

Enumeration

# UISplitViewController.SplitBehavior

Constants that describe the possible ways that the child view controllers appear in relation to each other.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum SplitBehavior
```

## Overview

A split view controller’s split behavior controls how its secondary view controller appears in relation to the others. You can configure this behavior so that the secondary view controller always appears side-by-side with the others, so that it’s partially obscured by the others, or so that it’s displaced offscreen opposite the others to make space for them.

A split view controller’s split behavior affects its possible display mode (displayMode). For more information, see UISplitViewController.DisplayMode.

| Split Behavior | Possible Display Modes |
|----|----|
| Tile | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneBesideSecondary  UISplitViewController.DisplayMode.twoBesideSecondary |
| Overlay | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneOverSecondary  UISplitViewController.DisplayMode.twoOverSecondary |
| Displace | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneBesideSecondary  UISplitViewController.DisplayMode.twoDisplaceSecondary |

## Topics

### Constants

case automatic

The split view controller automatically decides the most appropriate split behavior based on the device and the current app size.

case tile

The sidebars and secondary view controller appear tiled side-by-side.

case overlay

The sidebars are layered on top of the secondary view controller, leaving the secondary view controller partially visible.

case displace

The sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the split behavior

var preferredSplitBehavior: UISplitViewController.SplitBehavior

The preferred behavior that determines how the child view controllers appear in relation to each other.

var splitBehavior: UISplitViewController.SplitBehavior

The current behavior that determines how the child view controllers appear in relation to each other.

