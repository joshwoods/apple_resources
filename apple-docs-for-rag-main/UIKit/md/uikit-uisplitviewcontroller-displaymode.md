

- UIKit
- UISplitViewController
-  displayMode 

Instance Property

# displayMode

The current arrangement of the split view interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var displayMode: UISplitViewController.DisplayMode { get }
```

## Discussion

This property reflects the arrangement of the child view controllers in a split view interface. The value in this property is never set to UISplitViewController.DisplayMode.automatic. To change the current display mode, change the value of the preferredDisplayMode property. If you just want to change which columns are shown, consider using show(_:) or hide(_:) and the split view controller will determine how to update the display mode to display the desired columns.

When isCollapsed is true, the value of this property is ignored. A collapsed split view interface contains only one view controller, so the display mode is superfluous.

## See Also

### Managing the display mode

var preferredDisplayMode: UISplitViewController.DisplayMode

The preferred arrangement of the split view interface.

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

