

- AppKit
-  NSPopover 

Class

# NSPopover

A means to display additional content related to existing content on the screen.

macOS 10.7+

``` source
@MainActor
class NSPopover
```

## Overview

The popover is positioned relative to the existing content and an anchor is used to express the relation between these two units of content. A popover has an appearance that specifies its visual characteristics, as well as a behavior that determines which user interactions will cause the popover to close. A transient popover is closed in response to most user interactions, whereas a semi-transient popover is closed when the user interacts with the window containing the popover’s positioning view. Popovers with application-defined behavior are not usually closed on the developer’s behalf.

The system automatically positions each popover relative to its positioning view and moves the popover whenever its positioning view moves. A positioning rectangle within the positioning view can be specified for additional granularity.

Popovers can be detached to become a separate window when they are dragged by implementing the appropriate delegate method.

## Topics

### Accessing a Popover’s Content View Controller

var contentViewController: NSViewController?

The view controller that manages the content of the popover.

### Managing a Popover’s Position and Size

var behavior: NSPopover.Behavior

Specifies the behavior of the popover.

func show(relativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the popover anchored to the specified view.

var positioningRect: NSRect

The rectangle within the positioning view relative to which the popover should be positioned.

### Managing a Popover’s Appearance

var appearance: NSAppearance?

The appearance of the popover.

var effectiveAppearance: NSAppearance

The appearance that will be used when the popover is displayed onscreen.

var animates: Bool

Specifies if the popover is to be animated.

var contentSize: NSSize

The content size of the popover.

var isShown: Bool

The display state of the popover.

var isDetached: Bool

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

### Closing a Popover

func performClose(Any?)

Attempts to close the popover.

func close()

Forces the popover to close without consulting its delegate.

### Getting and Setting the Delegate

var delegate: (any NSPopoverDelegate)?

The delegate of the popover.

### Constants

enum Behavior

The appearance and disappearance behavior of a popover.

class let closeReasonUserInfoKey: String

The `userInfo` key containing the reason for the willCloseNotification.

struct CloseReason

Values that specify the reason for the willCloseNotification notification.

enum Appearance

The set of predefined appearances for a popover.

Deprecated

### Notifications

class let willShowNotification: NSNotification.Name

Sent before the popover is shown.

class let didShowNotification: NSNotification.Name

Sent after the popover has finished animating onscreen.

class let willCloseNotification: NSNotification.Name

Sent before the popover is closed.

class let didCloseNotification: NSNotification.Name

Sent after the popover has finished animating offscreen.

### Initializers

init()

init?(coder: NSCoder)

### Instance Properties

var hasFullSizeContent: Bool

A Boolean value that indicates whether the content view of the popover extends into the arrow region.

### Instance Methods

func show(relativeTo: NSToolbarItem)

Shows the popover anchored to the specified toolbar item.

## Relationships

### Inherits From

- NSResponder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAppearanceCustomization
- NSCoding
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable

## See Also

### Popovers

protocol NSPopoverDelegate

A set of optional methods that a popover delegate can implement to provide additional or custom functionality.

