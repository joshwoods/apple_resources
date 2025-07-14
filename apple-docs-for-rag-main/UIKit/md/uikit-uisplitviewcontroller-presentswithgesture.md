

- UIKit
- UISplitViewController
-  presentsWithGesture 

Instance Property

# presentsWithGesture

Specifies whether a hidden view controller can be presented and dismissed using a swipe gesture.

iOS 5.1+iPadOS 5.1+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var presentsWithGesture: Bool { get set }
```

## Discussion

When this property is true, the split view controller installs a gesture recognizer for changing the current display mode. In a column-style split view interface, the gesture is interactive.

In a classic split view interface, the gesture recognizer applies the display mode returned by the delegate’s targetDisplayModeForAction(in:) method. If that method returns the UISplitViewController.DisplayMode.automatic mode, the split view controller applies the most appropriate display mode given its current configuration and size class.

When this property is false, the split view controller doesn’t install a gesture recognizer for changing the display mode. The split view controller also doesn’t display a button to change the display mode.

The default value of this property is true.

## See Also

### Managing the display mode

var preferredDisplayMode: UISplitViewController.DisplayMode

The preferred arrangement of the split view interface.

var displayMode: UISplitViewController.DisplayMode

The current arrangement of the split view interface.

var displayModeButtonItem: UIBarButtonItem

A button that changes the display mode of the split view controller.

var showsSecondaryOnlyButton: Bool

Specifies whether the secondary view controller shows a button to toggle to and from the secondary-only display mode.

enum DisplayMode

Constants that describe the possible arrangements for a split view interface.

var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

enum DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

