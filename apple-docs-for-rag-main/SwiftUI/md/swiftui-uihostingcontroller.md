

- SwiftUI
-  UIHostingController 

Class

# UIHostingController

A UIKit view controller that manages a SwiftUI view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
class UIHostingController where Content : View
```

## Overview

Create a `UIHostingController` object when you want to integrate SwiftUI views into a UIKit view hierarchy. At creation time, specify the SwiftUI view you want to use as the root view for this view controller; you can change that view later using the rootView property. Use the hosting controller like you would any other view controller, by presenting it or embedding it as a child view controller in your interface.

## Topics

### Creating a hosting controller object

init(rootView: Content)

Creates a hosting controller object that wraps the specified SwiftUI view.

init?(coder: NSCoder, rootView: Content)

Creates a hosting controller object from an archive and the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting controller object from the contents of the specified archive.

### Responding to view-related events

func loadView()

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewDidAppear(Bool)

Notifies the view controller that its view has been added to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view will be removed from a view hierarchy.

func viewDidDisappear(Bool)

func willMove(toParent: UIViewController?)

func didMove(toParent: UIViewController?)

func viewWillTransition(to: CGSize, with: any UIViewControllerTransitionCoordinator)

func viewWillLayoutSubviews()

func target(forAction: Selector, withSender: Any?) -> Any?

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this view controller.

### Checking for modality

var isModalInPresentation: Bool

### Managing the size

var sizingOptions: UIHostingControllerSizingOptions

The options for how the hosting controller tracks changes to the size of its SwiftUI content.

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

### Configuring the status bar

var preferredStatusBarStyle: UIStatusBarStyle

The preferred status bar style for the view controller.

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

The animation style to use when hiding or showing the status bar for this view controller.

var prefersStatusBarHidden: Bool

A Boolean value that indicates whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarStyle: UIViewController?

var childForStatusBarHidden: UIViewController?

### Configuring the home indicator

var prefersHomeIndicatorAutoHidden: Bool

A Boolean value that indicates whether the view controller prefers the home indicator to be hidden or shown.

var childForHomeIndicatorAutoHidden: UIViewController?

### Configuring the interface appearance

var preferredUserInterfaceStyle: UIUserInterfaceStyle

The preferred interface style for this view controller.

var preferredScreenEdgesDeferringSystemGestures: UIRectEdge

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

var childForScreenEdgesDeferringSystemGestures: UIViewController?

### Accessing the available key commands

var keyCommands: [UIKeyCommand]?

### Managing undo

var undoManager: UndoManager?

### Instance Properties

var childViewControllerForPreferredContainerBackgroundStyle: UIViewController?

var preferredContainerBackgroundStyle: UIContainerBackgroundStyle

### Instance Methods

func addChild(UIViewController)

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Displaying SwiftUI views in UIKit

Using SwiftUI with UIKit

Learn how to incorporate SwiftUI views into a UIKit app.

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

struct UIHostingControllerSizingOptions

Options for how a hosting controller tracks its content’s size.

struct UIHostingConfiguration

A content configuration suitable for hosting a hierarchy of SwiftUI views.

