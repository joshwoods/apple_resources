

- UIKit
- UISplitViewController
-  preferredDisplayMode 

Instance Property

# preferredDisplayMode

The preferred arrangement of the split view interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredDisplayMode: UISplitViewController.DisplayMode { get set }
```

## Discussion

Use this property to specify the display mode that you prefer to use. The split view controller makes every effort to adopt the interface you specify, but may use a different type of interface if there isn’t enough space to support your preferred choice. If changing the value of this property leads to an actual change in the current display mode, the split view controller updates displayMode. The resulting change is animated if you made the change in an animation block.

Setting the value of this property to UISplitViewController.DisplayMode.automatic causes the split view controller to choose the most appropriate display mode for the currently available space. The default value of this property is UISplitViewController.DisplayMode.automatic.

A split view controller’s split behavior affects its possible display mode. The preferred display mode is interpreted to match the current splitBehavior. For example, if you set the preferred display mode to UISplitViewController.DisplayMode.twoBesideSecondary, the actual displayMode is interpreted as UISplitViewController.DisplayMode.twoOverSecondary for UISplitViewController.SplitBehavior.overlay, and as UISplitViewController.DisplayMode.twoDisplaceSecondary for UISplitViewController.SplitBehavior.displace.

If presentsWithGesture is false, the value of this property is strictly respected.

## See Also

### Managing the display mode

var displayMode: UISplitViewController.DisplayMode

The current arrangement of the split view interface.

var displayModeButtonItem: UIBarButtonItem

A button that changes the display mode of the split view controller.

var presentsWithGesture: Bool

Specifies whether a hidden view controller can be presented and dismissed using a swipe gesture.

var showsSecondaryOnlyButton: Bool

Specifies whether the secondary view controller shows a button to toggle to and from the secondary-only display mode.

enum DisplayMode

Constants that describe the possible arrangements for a split view interface.

var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

enum DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

