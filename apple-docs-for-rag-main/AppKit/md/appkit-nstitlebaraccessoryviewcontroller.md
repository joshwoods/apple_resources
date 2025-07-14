

- AppKit
-  NSTitlebarAccessoryViewController 

Class

# NSTitlebarAccessoryViewController

An object that manages a custom view—known as an accessory view—in the title bar–toolbar area of a window.

macOS 10.10+

``` source
@MainActor
class NSTitlebarAccessoryViewController
```

## Overview

Because a title bar accessory view controller is contained in a visual effect view (that is, NSVisualEffectView), it automatically handles the blur behind the accessory view and the size and location changes for the content of the view when a window goes in and out of full screen mode. If you’re currently using NSToolbar fullscreen accessory APIs, such as fullScreenAccessoryView, you should use NSTitlebarAccessoryViewController APIs instead.

Typically, you create an `NSTitlebarAccessoryViewController` object, give it your custom view, set the layoutAttribute property to ensure that it displays correctly in relation to the title bar, and add the view controller to your window. For more information about NSWindow methods you can use to add and remove a title bar accessory view controller, see Managing Title Bars.

Don’t override the `view` property in your `NSTitlebarAccessoryViewController` subclass. Instead, you can override loadView(), and set the `view` property in that method.

Note

`NSTitlebarAccessoryViewController` observes the view’s frame for changes. Depending on the value of layoutAttribute, you can change either the height or the width of the view. Specifically, you can change the view’s height when layoutAttribute is NSLayoutConstraint.Attribute.bottom, and you can change the view’s width when the layoutAttribute is NSLayoutConstraint.Attribute.right or NSLayoutConstraint.Attribute.left. The remaining size direction is automatically set to the maximum size as required for the window.

## Topics

### Configuring a Title Bar Accessory View Controller

var fullScreenMinHeight: CGFloat

The visual minimum height of an accessory view that displays below the title bar when the window is in full screen mode.

var layoutAttribute: NSLayoutConstraint.Attribute

The location of the accessory view, in relation to the window’s title bar.

### Responding to View Events

func viewDidAppear()

Called when the title bar accessory view controller’s view is fully transitioned onto the screen.

func viewDidDisappear()

Called after the title bar accessory view controller’s view is removed from the window’s view hierarchy.

func viewWillAppear()

Called after the title bar accessory view controller’s view has been loaded into memory is about to be added to the view hierarchy in the window.

### Instance Properties

var automaticallyAdjustsSize: Bool

var isHidden: Bool

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAnimatablePropertyContainer
- NSAnimationDelegate
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Content Controllers

class NSWindowController

A controller that manages a window, usually a window stored in a nib file.

class NSViewController

A controller that manages a view, typically loaded from a nib file.

