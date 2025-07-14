

- AppKit
-  NSForm Deprecated

Class

# NSForm

An `NSForm` object is a vertical matrix of NSFormCell objects to implement the fields.

macOS 10.0–10.10Deprecated

``` source
@MainActor
class NSForm
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Topics

### Adding and Removing Entries

func addEntry(String) -> NSFormCell

Adds a new entry to the end of the receiver and gives it the specified title.

func insertEntry(String, at: Int) -> NSFormCell!

Inserts an entry with the specified title into the receiver.

func removeEntry(at: Int)

Removes and releases the entry at the specified index.

### Changing the Appearance of All the Entries

func setBezeled(Bool)

Sets whether the receiver’s entries should display a bezel around their editable text.

func setBordered(Bool)

Sets whether the receiver’s entries should display a border around their editable text fields.

func setEntryWidth(CGFloat)

Sets the width of all the entries in the receiver.

func setFrameSize(NSSize)

Sets the size of the receiver’s frame size to the specified value.

func setInterlineSpacing(CGFloat)

Sets the spacing between entries

func setTitleAlignment(NSTextAlignment)

Sets the alignment for all of the entry titles.

func setTitleBaseWritingDirection(NSWritingDirection)

Sets the writing direction for the title of every control embedded in the form.

func setTextAlignment(NSTextAlignment)

Sets the alignment for all of the receiver’s editable text.

func setTextBaseWritingDirection(NSWritingDirection)

Sets the writing direction for the text content of every control embedded in the form.

func setTitleFont(NSFont)

Sets the font for all of the entry titles.

func setTextFont(NSFont)

Sets the font for all of the receiver’s editable text fields

### Getting Cells and Indices

func indexOfCell(withTag: Int) -> Int

Returns the index of the entry whose tag is `tag`.

func indexOfSelectedItem() -> Int

Returns the index of the selected entry.

func cell(at: Int) -> Any!

Returns the entry at the specified index.

### Displaying a Cell

func drawCell(at: Int)

Displays the entry at the specified index.

### Auto Layout Sizing

func preferredTextFieldWidth() -> CGFloat

The preferred width of the form’s cells when using Auto Layout.

func setPreferredTextFieldWidth(CGFloat)

Sets the preferred text field width used by Auto Layout.

### Editing Text

func selectText(at: Int)

Selects the entry at the specified index.

## Relationships

### Inherits From

- NSMatrix

### Conforms To

- CVarArg
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
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- NSViewToolTipOwner
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

class NSFormCell

The `NSFormCell` class is used to implement text entry fields in a form. The left part of an `NSFormCell` object contains a title. The right part contains an editable text entry field.

class NSMenuItemCell

An object that handles the measurement and display of a single menu item in its encompassing frame.

