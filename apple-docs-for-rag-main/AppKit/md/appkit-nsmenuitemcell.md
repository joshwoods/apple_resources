

- AppKit
-  NSMenuItemCell 

Class

# NSMenuItemCell

An object that handles the measurement and display of a single menu item in its encompassing frame.

macOS

``` source
@MainActor
class NSMenuItemCell
```

## Overview

Note

`NSMenuItemCell` is no longer used to draw menus. Using it does not affect the appearance of your menus.

## Topics

### Initializers

init(coder: NSCoder)

init(textCell: String)

### Configuring Menu-Item Attributes

var menuItem: NSMenuItem?

The menu item object associated with the cell.

### Calculating the Size of a Menu Item

func calcSize()

Calculates the minimum required width and height of the receiver’s menu item.

var needsSizing: Bool

A Boolean value indicating whether the size of the menu needs to be calculated.

var imageWidth: CGFloat

The width of the image associated with the menu item.

var titleWidth: CGFloat

The width of the menu item’s text, measured in points.

var keyEquivalentWidth: CGFloat

The width of the menu item’s key equivalent string.

var stateImageWidth: CGFloat

The width of the image used to indicate the state of the menu item.

### Getting the Menu Item’s Drawing Rectangle

func keyEquivalentRect(forBounds: NSRect) -> NSRect

Returns the rectangle into which the menu item’s key equivalent should be drawn.

func stateImageRect(forBounds: NSRect) -> NSRect

Returns the rectangle into which the menu item’s state image should be drawn.

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle into which the menu item’s title should be drawn.

### Drawing the Menu Item

func drawBorderAndBackground(withFrame: NSRect, in: NSView)

Draws the borders and background associated with the receiver’s menu item (if any).

func drawImage(withFrame: NSRect, in: NSView)

Draws the image associated with the menu item.

func drawKeyEquivalent(withFrame: NSRect, in: NSView)

Draws the key equivalent associated with the menu item.

func drawSeparatorItem(withFrame: NSRect, in: NSView)

Draws a menu item separator.

func drawStateImage(withFrame: NSRect, in: NSView)

Draws the state image associated with the menu item.

func drawTitle(withFrame: NSRect, in: NSView)

Draws the title associated with the menu item.

var needsDisplay: Bool

A Boolean value indicating whether the menu item needs to be displayed.

### Assigning a Tag

var tag: Int

The integer tag of the selected menu item.

## Relationships

### Inherits From

- NSButtonCell

### Inherited By

- NSPopUpButtonCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
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

class NSDrawer

A user interface element that contains and displays text, scroll, and browser views, in addition to other view subclasses.

Deprecated

class NSForm

An `NSForm` object is a vertical matrix of NSFormCell objects to implement the fields.

Deprecated

class NSFormCell

The `NSFormCell` class is used to implement text entry fields in a form. The left part of an `NSFormCell` object contains a title. The right part contains an editable text entry field.

