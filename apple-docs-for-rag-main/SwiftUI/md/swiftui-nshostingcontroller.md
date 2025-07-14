

- SwiftUI
-  NSHostingController 

Class

# NSHostingController

An AppKit view controller that hosts SwiftUI view hierarchy.

macOS 10.15+

``` source
@MainActor @preconcurrency
class NSHostingController where Content : View
```

## Overview

Create an `NSHostingController` object when you want to integrate SwiftUI views into an AppKit view hierarchy. At creation time, specify the SwiftUI view you want to use as the root view for this view controller; you can change that view later using the rootView property. Use the hosting controller like you would any other view controller, by presenting it or embedding it as a child view controller in your interface.

## Topics

### Creating a hosting controller object

init(rootView: Content)

Creates a hosting controller object that wraps the specified SwiftUI view.

init?(coder: NSCoder, rootView: Content)

Creates a hosting controller object from an archive and the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting controller object from the contents of the specified archive.

### Getting the root view

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this view controller.

var identifier: NSUserInterfaceItemIdentifier?

### Configuring the controller

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var preferredContentSize: NSSize

var sizingOptions: NSHostingSizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Displaying SwiftUI views in AppKit

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class NSHostingView

An AppKit view that hosts a SwiftUI view hierarchy.

class NSHostingMenu

An AppKit menu with menu items that are defined by a SwiftUI View.

struct NSHostingSizingOptions

Options for how hosting views and controllers reflect their content’s size into Auto Layout constraints.

struct NSHostingSceneBridgingOptions

Options for how hosting views and controllers manage aspects of the associated window.

