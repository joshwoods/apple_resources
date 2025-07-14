

- AppKit
-  NSFormCell 

Class

# NSFormCell

The `NSFormCell` class is used to implement text entry fields in a form. The left part of an `NSFormCell` object contains a title. The right part contains an editable text entry field.

macOS

``` source
@MainActor
class NSFormCell
```

## Overview

An `NSFormCell` object implements the user interface of an NSForm object.

## Topics

### Initializers

init(coder: NSCoder)

### Initializing an NSFormCell

init(textCell: String?)

Returns an `NSFormCell` object initialized with the specified title string.

### Asking About a Cell’s Appearance

var isOpaque: Bool

A Boolean value indicating whether the title is empty and an opaque bezel is set.

### Accessing a Cell’s Title

var attributedTitle: NSAttributedString

The title of the cell as an attributed string.

var title: String

The cell’s title text.

var titleAlignment: NSTextAlignment

The alignment of the title.

var titleBaseWritingDirection: NSWritingDirection

The default writing direction used to render the form cell’s title.

var titleFont: NSFont

The font used to draw cell’s title.

var titleWidth: CGFloat

The width of the title field.

### Asking About Placeholder Values

var placeholderAttributedString: NSAttributedString?

The cell’s attributed placeholder string.

var placeholderString: String?

The cell’s plain text placeholder string.

### Sizing for Auto Layout

var preferredTextFieldWidth: CGFloat

The preferred text field width.

### Instance Methods

func titleWidth(NSSize) -> CGFloat

Returns the width of the title field constrained to the specified size.

## Relationships

### Inherits From

- NSActionCell

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

class NSMenuItemCell

An object that handles the measurement and display of a single menu item in its encompassing frame.

