

- AppKit
-  NSTokenFieldCellDelegate 

Protocol

# NSTokenFieldCellDelegate

A set of optional methods implemented by delegates of NSTokenFieldCell objects to work with tokenized strings.

macOS

``` source
protocol NSTokenFieldCellDelegate : NSObjectProtocol
```

## Topics

### Displaying Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, displayStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be displayed as a proxy for the represented object.

func tokenFieldCell(NSTokenFieldCell, styleForRepresentedObject: Any) -> NSTokenField.TokenStyle

Allows the delegate to return the token style for editing the specified represented object.

### Editing a Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [Any]

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenFieldCell(NSTokenFieldCell, editingStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be edited as a proxy for the represented object.

func tokenFieldCell(NSTokenFieldCell, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the string being edited.

func tokenFieldCell(NSTokenFieldCell, shouldAdd: [Any], at: Int) -> [Any]

Allows the delegate to validate the tokens to be added to the receiver at a given index.

### Reading To and Writing From the Pasteboard

func tokenFieldCell(NSTokenFieldCell, readFrom: NSPasteboard) -> [Any]?

Allows the delegate to return an array of objects representing the data read from `pboard`.

func tokenFieldCell(NSTokenFieldCell, writeRepresentedObjects: [Any], to: NSPasteboard) -> Bool

Allows the delegate the opportunity to write custom pasteboard types to the pasteboard for the represented objects in `objects`.

### Managing Menus for Represented Objects

func tokenFieldCell(NSTokenFieldCell, hasMenuForRepresentedObject: Any) -> Bool

Allows the delegate to specify whether the represented object provides a menu.

func tokenFieldCell(NSTokenFieldCell, menuForRepresentedObject: Any) -> NSMenu?

Allows the delegate to provide a menu for the specified represented object.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Cell

class NSTokenFieldCell

A text field cell subclass that enables tokenized editing of an array of objects.

