

- UIKit
- UISplitViewController
-  UISplitViewController.DisplayMode 

Enumeration

# UISplitViewController.DisplayMode

Constants that describe the possible arrangements for a split view interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum DisplayMode
```

## Overview

A split view controller’s display mode controls the visual arrangement of its child view controllers. You set a preferred display mode by using the preferredDisplayMode property, and the split view controller updates itself and reflects the actual display mode in the displayMode property.

Display modes apply to a split view controller in an expanded arrangement. When the split view interface is collapsed — when isCollapsed is true — the display mode has no impact on the appearance of the split view controller interface.

A split view controller’s split behavior (splitBehavior) affects its possible display modes. For more information, see UISplitViewController.SplitBehavior.

| Split Behavior | Possible Display Modes |
|----|----|
| Tile | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneBesideSecondary  UISplitViewController.DisplayMode.twoBesideSecondary |
| Overlay | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneOverSecondary  UISplitViewController.DisplayMode.twoOverSecondary |
| Displace | UISplitViewController.DisplayMode.secondaryOnly  UISplitViewController.DisplayMode.oneBesideSecondary  UISplitViewController.DisplayMode.twoDisplaceSecondary |

There are several ways for user interaction to change the current display mode. Based on the type of user interaction (gesture or button tap), the display mode can transition between a set of predetermined states.

## Topics

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

case twoDisplaceSecondary

Two sidebars displace the secondary view controller instead of overlapping it, moving it partially offscreen.

### Deprecated

static var primaryHidden: UISplitViewController.DisplayMode

The primary view controller is hidden.

Deprecated

static var allVisible: UISplitViewController.DisplayMode

The primary and secondary view controllers are displayed side-by-side onscreen.

Deprecated

static var primaryOverlay: UISplitViewController.DisplayMode

The primary view controller is layered on top of the secondary view controller, leaving the secondary view controller partially visible.

Deprecated

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

### Managing the display mode

var preferredDisplayMode: UISplitViewController.DisplayMode

The preferred arrangement of the split view interface.

var displayMode: UISplitViewController.DisplayMode

The current arrangement of the split view interface.

var displayModeButtonItem: UIBarButtonItem

A button that changes the display mode of the split view controller.

var presentsWithGesture: Bool

Specifies whether a hidden view controller can be presented and dismissed using a swipe gesture.

var showsSecondaryOnlyButton: Bool

Specifies whether the secondary view controller shows a button to toggle to and from the secondary-only display mode.

var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

enum DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

