

- AppKit
-  NSTextFieldCell 

Class

# NSTextFieldCell

An object that enhances the text display capabilities of a cell.

macOS

``` source
@MainActor
class NSTextFieldCell
```

## Overview

The NSTextFieldCell class adds to the text display capabilities of the NSCell class by allowing you to set the color of both the text and its background. You can also specify whether the cell draws its background at all.

All of the methods declared by this class are also declared by the NSTextField class, which uses NSTextFieldCell objects to draw and edit text. The NSTextField cover methods call the corresponding NSTextFieldCell methods.

Placeholder strings, set using the placeholderString or placeholderAttributedString property, appear in the text field cell if the actual string is `nil` or an empty string. They’re drawn in gray on the cell and aren’t archived in the “pre-10.2” nib format.

### Designated Initializers

When subclassing `NSTextFieldCell` you must implement the designated initializers init(coder:) and init(textCell:).

## Topics

### Creating a Text Field Cell

init(textCell: String)

Initializes a text field cell that displays the specified string.

init(coder: NSCoder)

Initializes a text field cell from data in the provided unarchiver.

### Setting the Text Color

var textColor: NSColor?

The color to use to draw the cell’s text.

### Setting the Bezel Style

var bezelStyle: NSTextField.BezelStyle

The bezel style to use when drawing the text field.

enum BezelStyle

The style of bezel the text field displays.

### Controlling the Background

var backgroundColor: NSColor?

The color of the cell’s background.

var drawsBackground: Bool

A Boolean value that indicates whether the cell draws its background color.

### Managing the Field Editor

func setUpFieldEditorAttributes(NSText) -> NSText

Allows the cell to set up the field editor’s attributes before editing begins.

func setWantsNotificationForMarkedText(Bool)

Directs the cell’s associated field editor to post text change notifications.

### Managing Placeholder Strings

var placeholderString: String?

The placeholder text for the cell, specified as a plain text string.

var placeholderAttributedString: NSAttributedString?

The placeholder text for the cell, specified as an attributed string.

### Accessing Input Source Locales

var allowedInputSourceLocales: [String]?

An array of locale identifiers that represent the allowed input sources when the text field has the keyboard focus.

## Relationships

### Inherits From

- NSActionCell

### Inherited By

- NSComboBoxCell
- NSPathComponentCell
- NSSearchFieldCell
- NSSecureTextFieldCell
- NSTableHeaderCell
- NSTokenFieldCell

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

### Cell

class NSSecureTextFieldCell

A text field whose value is hidden from the user.

