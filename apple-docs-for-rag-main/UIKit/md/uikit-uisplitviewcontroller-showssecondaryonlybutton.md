

- UIKit
- UISplitViewController
-  showsSecondaryOnlyButton 

Instance Property

# showsSecondaryOnlyButton

Specifies whether the secondary view controller shows a button to toggle to and from the secondary-only display mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
@MainActor
var showsSecondaryOnlyButton: Bool { get set }
```

## Discussion

This value only takes effect when the split view controller’s style property is UISplitViewController.Style.tripleColumn.

The default value of this property is false. If you set the value to true, the secondary view controller shows a button that lets a user toggle the display mode to and from UISplitViewController.DisplayMode.secondaryOnly.

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

enum DisplayMode

Constants that describe the possible arrangements for a split view interface.

var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

enum DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

