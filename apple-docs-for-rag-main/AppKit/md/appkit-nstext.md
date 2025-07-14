

- AppKit
-  NSText 

Class

# NSText

The most general programmatic interface for objects that manage text.

macOS

``` source
@MainActor
class NSText
```

## Overview

NSText draws text for user interface objects, provides text editing capabilities, and controls text attributes such as type size, font, and color.

NSText initialization creates an instance of a concrete subclass, such as NSTextView (generically called a text object). In general, you’re more likely to use the NSTextView subclass, because it extends the interface declared by NSText and provides much more sophisticated functionality than that declared in NSText.

AppKit uses text objects wherever text appears in interface objects. For example, a text object draws the title of a window, the commands in a menu, the title of a button, and the items in a browser. Your app can also create text objects for its own purposes.

## Topics

### Creating a Text Object

init?(coder: NSCoder)

init(frame: NSRect)

### Getting the characters

var string: String

The characters of the receiver’s text.

### Setting graphics attributes

var backgroundColor: NSColor?

The receiver’s background color to a given color.

var drawsBackground: Bool

A Boolean that controls whether the receiver draws its background.

### Setting behavioral attributes

var isEditable: Bool

A Boolean that controls whether the receiver allows the user to edit its text.

var isSelectable: Bool

A Boolean that controls whether the receiver allows the user to select its text.

var isFieldEditor: Bool

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

var isRichText: Bool

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

var importsGraphics: Bool

A Boolean that controls whether the receiver allows the user to import files by dragging.

### Using the Font panel and menu

var usesFontPanel: Bool

A Boolean that controls whether the receiver uses the Font panel and Font menu.

### Using the ruler

func toggleRuler(Any?)

This action method shows or hides the ruler, if the receiver is enclosed in a scroll view.

var isRulerVisible: Bool

A Boolean value that indicates whether the receiver’s enclosing scroll view shows its ruler.

### Changing the selection

var selectedRange: NSRange

The receiver’s characters within `aRange`.

### Replacing text

func replaceCharacters(in: NSRange, withRTF: Data)

Replaces the characters in the given range with RTF text interpreted from the given RTF data.

func replaceCharacters(in: NSRange, withRTFD: Data)

Replaces the characters in the given range with RTFD text interpreted from the given RTFD data.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters in the given range with those in the given string.

### Action methods for editing

func selectAll(Any?)

This action method selects all of the receiver’s text.

func copy(Any?)

This action method copies the selected text onto the general pasteboard, in as many formats as the receiver supports.

func cut(Any?)

This action method deletes the selected text and places it onto the general pasteboard, in as many formats as the receiver supports.

func paste(Any?)

This action method pastes text from the general pasteboard at the insertion point or over the selection.

func copyFont(Any?)

This action method copies the font information for the first character of the selection (or for the insertion point) onto the font pasteboard, as `NSFontPboardType`.

func pasteFont(Any?)

This action method pastes font information from the font pasteboard onto the selected text or insertion point of a rich text object, or over all text of a plain text object.

func copyRuler(Any?)

This action method copies the paragraph style information for first selected paragraph onto the ruler pasteboard, as `NSRulerPboardType`, and expands the selection to paragraph boundaries.

func pasteRuler(Any?)

This action method pastes paragraph style information from the ruler pasteboard onto the selected paragraphs of a rich text object.

func delete(Any?)

This action method deletes the selected text.

### Changing the font

func changeFont(Any?)

This action method changes the font of the selection for a rich text object, or of all text for a plain text object.

var font: NSFont?

The font of all the receiver’s text.

func setFont(NSFont, range: NSRange)

Sets the font of characters within `aRange` to `aFont`.

### Setting text alignment

var alignment: NSTextAlignment

The alignment of all the receiver’s text.

func alignCenter(Any?)

This action method applies center alignment to selected paragraphs (or all text if the receiver is a plain text object).

func alignLeft(Any?)

This action method applies left alignment to selected paragraphs (or all text if the receiver is a plain text object).

func alignRight(Any?)

This action method applies right alignment to selected paragraphs (or all text if the receiver is a plain text object).

### Setting text color

var textColor: NSColor?

The text color of all characters in the receiver.

func setTextColor(NSColor?, range: NSRange)

Sets the text color of characters within the specified range to the specified color.

### Writing direction

var baseWritingDirection: NSWritingDirection

The initial writing direction used to determine the actual writing direction for text.

### Setting superscripting and subscripting

func superscript(Any?)

This action method applies a superscript attribute to selected text (or all text if the receiver is a plain text object), raising its baseline offset by a predefined amount.

func `subscript`(Any?)

This action method applies a subscript attribute to selected text (or all text if the receiver is a plain text object), lowering its baseline offset by a predefined amount.

func unscript(Any?)

This action method removes any superscripting or subscripting from selected text (or all text if the receiver is a plain text object).

### Underlining text

func underline(Any?)

Adds the underline attribute to the selected text attributes if absent; removes the attribute if present.

### Reading and writing RTF files

func readRTFD(fromFile: String) -> Bool

Attempts to read the RTFD file at `path`, returning true if successful and false if not.

func writeRTFD(toFile: String, atomically: Bool) -> Bool

Writes the receiver’s text as RTF with attachments to a file or directory at `path`.

func rtfd(from: NSRange) -> Data?

Returns an NSData object that contains an RTFD stream corresponding to the characters and attributes within `aRange`.

func rtf(from: NSRange) -> Data?

Returns an NSData object that contains an RTF stream corresponding to the characters and attributes within `aRange`, omitting any attachment characters and attributes.

### Checking spelling

func checkSpelling(Any?)

This action method searches for a misspelled word in the receiver’s text.

func showGuessPanel(Any?)

This action method opens the Spelling panel, allowing the user to make a correction during spell checking.

### Constraining size

var maxSize: NSSize

The receiver’s maximum size.

var minSize: NSSize

The receiver’s minimum size.

var isVerticallyResizable: Bool

A Boolean that controls whether the receiver changes its height to fit the height of its text.

var isHorizontallyResizable: Bool

A Boolean that controls whether the receiver changes its width to fit the width of its text.

func sizeToFit()

Resizes the receiver to fit its text.

### Scrolling

func scrollRangeToVisible(NSRange)

Scrolls the receiver in its enclosing scroll view so the first characters of `aRange` are visible.

### Setting the delegate

var delegate: (any NSTextDelegate)?

The receiver’s delegate.

### Constants

enum NSTextAlignment

Constants that specify text alignment.

enum NSWritingDirection

Constants that specify the writing direction.

Movement Codes

The reason for a change of editing focus among text fields.

Common Unicode Characters

### Notifications

class let didBeginEditingNotification: NSNotification.Name

Posted when an `NSText` object begins any operation that changes characters or formatting attributes.

class let didChangeNotification: NSNotification.Name

Posted after an `NSText` object performs any operation that changes characters or formatting attributes.

class let didEndEditingNotification: NSNotification.Name

Posted when focus leaves an `NSText` object, whether or not any operation has changed characters or formatting attributes.

class let movementUserInfoKey: String

The `userInfo` dictionary key for the didEndEditingNotification notification.

enum NSTextMovement

## Relationships

### Inherits From

- NSView

### Inherited By

- NSTextView

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
- NSChangeSpelling
- NSCoding
- NSDraggingDestination
- NSIgnoreMisspelledWords
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Text views

class NSTextField

Text the user can select or edit to send an action message to a target when the user presses the Return key.

protocol NSTextFieldDelegate

A protocol that a text field delegate can use to control its field editor action menu.

class NSTextView

A view that draws text and handles user interactions with that text.

protocol NSTextViewDelegate

A set of optional methods that text view delegates can use to manage selection, set text attributes, work with the spell checker, and more.

protocol NSTextDelegate

A set of optional methods implemented by the delegate of an NSText object to edit text and change text formats.

