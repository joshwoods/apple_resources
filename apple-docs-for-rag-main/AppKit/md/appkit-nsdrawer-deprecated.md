

- AppKit
-  NSDrawer Deprecated

Class

# NSDrawer

A user interface element that contains and displays text, scroll, and browser views, in addition to other view subclasses.

macOS 10.0–10.13Deprecated

``` source
@MainActor
class NSDrawer
```

Deprecated

Drawers are deprecated and should not be used in modern macOS apps.

## Overview

A drawer is associated with a window, called its parent, and can appear only while its parent is visible onscreen. A drawer cannot be moved or ordered independently of a window, but is instead attached to one edge of its parent and moves along with it.

## Topics

### Creating Drawers

init(contentSize: NSSize, preferredEdge: NSRectEdge)

Creates a new drawer with the given size on the specified edge of the parent window.

var delegate: (any NSDrawerDelegate)?

The receiver’s delegate.

### Opening and Closing Drawers

func close()

If the receiver is open, this method closes it.

func close(Any?)

An action method to close the receiver.

func open()

If the receiver is closed, this method opens it.

func open(Any?)

An action method to open the drawer.

func open(on: NSRectEdge)

Causes the receiver to open on the specified edge of the parent window.

func toggle(Any?)

Toggles the drawer open or closed.

var state: Int

The state of the receiver.

### Managing Drawer Size

var contentSize: NSSize

The size of the receiver’s content area.

var leadingOffset: CGFloat

The receiver’s leading offset.

var maxContentSize: NSSize

The maximum allowed size of the receiver’s content area.

var minContentSize: NSSize

The minimum allowed size of the receiver’s content area.

var trailingOffset: CGFloat

The receiver’s trailing offset.

### Managing Drawer Edges

var edge: NSRectEdge

The edge of the window that the receiver is connected to.

var preferredEdge: NSRectEdge

The receiver’s preferred, or default, edge.

### Managing Drawer Views

var contentView: NSView?

The receiver’s content view.

var parentWindow: NSWindow?

The receiver’s parent window.

### Constants

enum State

These constants specify the possible states of a drawer.

### Notifications

class let didCloseNotification: NSNotification.Name

Posted whenever the drawer is closed.

class let didOpenNotification: NSNotification.Name

Posted whenever the drawer is opened.

class let willCloseNotification: NSNotification.Name

Posted whenever the drawer is about to close.

class let willOpenNotification: NSNotification.Name

Posted whenever the drawer is about to open.

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
- NSCoding
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable

## See Also

### Classes

class NSOpenGLView

A view that displays OpenGL content in a view.

Deprecated

class NSOpenGLContext

An object that represents an OpenGL graphics context, into which all OpenGL calls are rendered.

Deprecated

class NSOpenGLLayer

A subclass of CAOpenGLLayer that is suitable for rendering OpenGL into layers.

Deprecated

class NSOpenGLPixelFormat

An object that specifies the types of buffers and other attributes of the OpenGL context.

Deprecated

class NSForm

An `NSForm` object is a vertical matrix of NSFormCell objects to implement the fields.

Deprecated

class NSFormCell

The `NSFormCell` class is used to implement text entry fields in a form. The left part of an `NSFormCell` object contains a title. The right part contains an editable text entry field.

class NSMenuItemCell

An object that handles the measurement and display of a single menu item in its encompassing frame.

