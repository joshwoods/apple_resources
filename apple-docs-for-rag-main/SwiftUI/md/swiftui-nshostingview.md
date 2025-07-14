

- SwiftUI
-  NSHostingView 

Class

# NSHostingView

An AppKit view that hosts a SwiftUI view hierarchy.

macOS 10.15+

``` source
@MainActor @preconcurrency
class NSHostingView where Content : View
```

## Overview

You use `NSHostingView` objects to integrate SwiftUI views into your AppKit view hierarchies. A hosting view is an NSView object that manages a single SwiftUI view, which may itself contain other SwiftUI views. Because it is an NSView object, you can integrate it into your existing AppKit view hierarchies to implement portions of your UI. For example, you can use a hosting view to implement a custom control.

A hosting view acts as a bridge between your SwiftUI views and your AppKit interface. During layout, the hosting view reports the content size preferences of your SwiftUI views back to the AppKit layout system so that it can size the view appropriately. The hosting view also coordinates event delivery.

## Topics

### Creating a hosting view

init(rootView: Content)

Creates a hosting view object that wraps the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting view object from the contents of the specified archive.

func prepareForReuse()

### Getting the root view

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this view controller.

### Configuring the view layout behavior

class var requiresConstraintBasedLayout: Bool

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

var isFlipped: Bool

var layerContentsRedrawPolicy: NSView.LayerContentsRedrawPolicy

func updateConstraints()

func layout()

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

### Managing keyboard interaction

func keyDown(with: NSEvent)

Called when the user presses a key on the keyboard while this view is in the responder chain.

func keyUp(with: NSEvent)

Called when the user releases a key on the keyboard while this view is in the responder chain.

func performKeyEquivalent(with: NSEvent) -> Bool

func insertText(Any)

func didChangeValue(forKey: String)

func makeTouchBar() -> NSTouchBar?

### Responding to mouse events

func mouseDown(with: NSEvent)

func mouseUp(with: NSEvent)

func otherMouseDown(with: NSEvent)

func otherMouseUp(with: NSEvent)

func rightMouseDown(with: NSEvent)

func rightMouseUp(with: NSEvent)

func mouseEntered(with: NSEvent)

func mouseExited(with: NSEvent)

func mouseDragged(with: NSEvent)

func mouseMoved(with: NSEvent)

func otherMouseDragged(with: NSEvent)

func rightMouseDragged(with: NSEvent)

func cursorUpdate(with: NSEvent)

### Responding to touch events

func touchesBegan(with: NSEvent)

func touchesCancelled(with: NSEvent)

func touchesEnded(with: NSEvent)

func touchesMoved(with: NSEvent)

### Responding to gestures

func magnify(with: NSEvent)

func rotate(with: NSEvent)

func scrollWheel(with: NSEvent)

### Handling drag and drop

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

### Providing a context menu

func menu(for: NSEvent) -> NSMenu?

### Responding to actions

func responds(to: Selector!) -> Bool

func forwardingTarget(for: Selector!) -> Any?

func doCommand(by: Selector)

### Configuring the responder behavior

var acceptsFirstResponder: Bool

var needsPanelToBecomeKey: Bool

### Managing the view hierarchy

func viewWillMove(toWindow: NSWindow?)

func viewDidMoveToWindow()

func viewDidChangeBackingProperties()

func viewDidChangeEffectiveAppearance()

### Modifying the frame rectangle

var intrinsicContentSize: NSSize

func setFrameSize(NSSize)

var firstBaselineOffsetFromTop: CGFloat

var lastBaselineOffsetFromBottom: CGFloat

var sizingOptions: NSHostingSizingOptions

The options for how the hosting view creates and updates constraints based on the size of its SwiftUI content.

var firstTextLineCenter: CGFloat?

### Testing for hits

func hitTest(NSPoint) -> NSView?

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

### Bridging with SwiftUI

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this hosting view.

### Initializers

init?(coder: NSCoder, rootView: Content)

Creates a hosting view object from an archive and the specified SwiftUI view.

### Instance Properties

var clipsToBounds: Bool

### Instance Methods

func acceptsFirstMouse(for: NSEvent?) -> Bool

func didAddSubview(NSView)

func observeValue(forKeyPath: String?, of: Any?, change: [NSKeyValueChangeKey : Any]?, context: UnsafeMutableRawPointer?)

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

func showContextMenuForSelection(Any?)

func willRemoveSubview(NSView)

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSDraggingSource
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations

## See Also

### Displaying SwiftUI views in AppKit

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class NSHostingController

An AppKit view controller that hosts SwiftUI view hierarchy.

class NSHostingMenu

An AppKit menu with menu items that are defined by a SwiftUI View.

struct NSHostingSizingOptions

Options for how hosting views and controllers reflect their content’s size into Auto Layout constraints.

struct NSHostingSceneBridgingOptions

Options for how hosting views and controllers manage aspects of the associated window.

