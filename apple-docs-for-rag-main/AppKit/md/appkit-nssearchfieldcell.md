

- AppKit
-  NSSearchFieldCell 

Class

# NSSearchFieldCell

The programmatic interface for text fields that are used for text-based searches.

macOS

``` source
@MainActor
class NSSearchFieldCell
```

## Overview

The NSSearchFieldCell class defines the programmatic interface for text fields that are optimized for text-based searches. An NSSearchFieldCell object is “wrapped” by an NSSearchField control object, which directly inherits from the NSTextField class. The search field implemented by these classes presents a standard user interface for searches, including a search button, a cancel button, and a pop-up icon menu for listing recent search strings and custom search categories.

When the user types and then pauses, the cell’s action message is sent to its target. You can query the cell’s string value for the current text to search for. Do not rely on the sender of the action to be an NSMenu object because the menu may change. If you need to change the menu, modify the search menu template and update the value in the searchMenuTemplate property.

## Topics

### Managing buttons

var searchButtonCell: NSButtonCell?

The button cell used to display the search-button image.

func resetSearchButtonCell()

Resets the search button cell to its default attributes.

var cancelButtonCell: NSButtonCell?

The button cell used to display the cancel-button image.

func resetCancelButtonCell()

Resets the cancel button cell to its default attributes.

### Custom layout

func searchTextRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search-text field cell.

func searchButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search button cell.

func cancelButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the cancel button cell.

### Managing menu templates

var searchMenuTemplate: NSMenu?

The menu object used to dynamically construct the search field’s pop-up icon menu.

### Managing search modes

var sendsWholeSearchString: Bool

A Boolean value indicating whether the cell calls its search action method when the user clicks the search button (or presses Return) or after each keystroke.

var sendsSearchStringImmediately: Bool

A Boolean value indicating whether the cell calls its action method immediately when an appropriate action occurs.

### Managing recent search strings

var maximumRecents: Int

The maximum number of search strings that can appear in the search menu.

var recentSearches: [String]!

An array of the recent search strings to display in the pop-up icon menu of the search field.

var recentsAutosaveName: NSSearchField.RecentsAutosaveName?

The autosave name under which the search field automatically saves the list of recent search strings.

### Constants

Menu tags

Constants for identifying special menu items in the search-menu template.

### Initializers

init(coder: NSCoder)

init(textCell: String)

## Relationships

### Inherits From

- NSTextFieldCell

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

