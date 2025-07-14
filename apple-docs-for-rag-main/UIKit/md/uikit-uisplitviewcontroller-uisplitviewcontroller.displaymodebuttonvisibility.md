

- UIKit
- UISplitViewController
-  UISplitViewController.DisplayModeButtonVisibility 

Enumeration

# UISplitViewController.DisplayModeButtonVisibility

Constants that determine the visibility of the display mode button.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+tvOS 14.5+visionOS 1.0+

``` source
enum DisplayModeButtonVisibility
```

## Topics

### Constants

case automatic

A constant that automatically determines the visibility of the display mode button.

case never

A constant that prevents the display mode button from appearing.

case always

A constant that allows the display mode button to always appear.

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

enum DisplayMode

Constants that describe the possible arrangements for a split view interface.

var displayModeButtonVisibility: UISplitViewController.DisplayModeButtonVisibility

A setting that determines whether the display mode button is visible in the interface.

