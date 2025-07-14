

- AppKit
-  NSTokenFieldDelegate 

Protocol

# NSTokenFieldDelegate

A set of optional methods implemented by delegates of NSTokenField objects.

macOS

``` source
protocol NSTokenFieldDelegate : NSTextFieldDelegate
```

## Topics

### Displaying Tokenized Strings

func tokenField(NSTokenField, displayStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be displayed as a proxy for the given represented object.

func tokenField(NSTokenField, styleForRepresentedObject: Any) -> NSTokenField.TokenStyle

Allows the delegate to return the token style for editing the specified represented object.

### Editing a Tokenized Strings

func tokenField(NSTokenField, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>?) -> [Any]?

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenField(NSTokenField, editingStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be edited as a proxy for a represented object.

func tokenField(NSTokenField, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the given editing string.

func tokenField(NSTokenField, shouldAdd: [Any], at: Int) -> [Any]

Allows the delegate to validate the tokens to be added to the receiver at a particular location.

### Reading To and Writing From the Pasteboard

func tokenField(NSTokenField, readFrom: NSPasteboard) -> [Any]?

Allows the delegate to return an array of objects representing the data read from the specified pasteboard.

func tokenField(NSTokenField, writeRepresentedObjects: [Any], to: NSPasteboard) -> Bool

Sent so the delegate can write represented objects to the pasteboard corresponding to a given array of display strings.

### Managing Menus for Represented Objects

func tokenField(NSTokenField, hasMenuForRepresentedObject: Any) -> Bool

Allows the delegate to specify whether the given represented object provides a menu.

func tokenField(NSTokenField, menuForRepresentedObject: Any) -> NSMenu?

Allows the delegate to provide a menu for the specified represented object.

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol
- NSTextFieldDelegate

