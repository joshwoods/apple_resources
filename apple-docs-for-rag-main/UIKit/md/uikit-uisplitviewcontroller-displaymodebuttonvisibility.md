

- UIKit
- UISplitViewController
-  displayModeButtonVisibility 

Instance Property

# displayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+tvOS 14.5+

``` source
@MainActor
var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility { get set }
```

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

enum DisplayMode

Constants that describe the possible arrangements for a split view interface.

enum DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

