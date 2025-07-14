

- AppKit
-  NSSearchField 

Class

# NSSearchField

A text field optimized for performing text-based searches.

macOS

``` source
@MainActor
class NSSearchField
```

## Overview

NSSearchField provides a customized text field for entering search data. The class also provides a search button, a cancel button, and a pop-up icon menu for listing recent search strings and custom search categories.

An NSSearchField object wraps an NSSearchFieldCell object. The cell provides access to most search field attributes and a comprehensive programmatic interface for manipulating the search field. You can use an NSSearchField object to manipulate some aspects of the search field.

For additional information about search fields and how to implement them, see the NSSearchFieldCell class.

## Topics

### Managing Search

var delegate: (any NSSearchFieldDelegate)?

The delegate for the search field, or `nil` if the search field doesn’t have a delegate.

protocol NSSearchFieldDelegate

A protocol that a search field delegate can use to determine when a search started or ended.

### Managing Menu Templates

var searchMenuTemplate: NSMenu?

The menu object used to dynamically construct the search field’s pop-up icon menu.

class let clearRecentsMenuItemTag: Int

The menu item for clearing the current set of recent string searches in the menu.

class let noRecentsMenuItemTag: Int

The menu item that describes a lack of recent search strings.

class let recentsMenuItemTag: Int

The location of recent search strings in the “recents” menu group.

class let recentsTitleMenuItemTag: Int

The menu item that provides the title of the menu group for recent search strings.

### Managing Search Modes

var sendsSearchStringImmediately: Bool

A Boolean value indicating whether the cell calls its action method immediately when an appropriate action occurs.

var sendsWholeSearchString: Bool

A Boolean value indicating whether the cell calls its search action method when the user clicks the search button or presses Return, or after each keystroke.

### Managing Recent Searches

var recentSearches: [String]

The list of recent search strings for the control.

var maximumRecents: Int

The maximum number of search strings that can appear in the search menu.

var recentsAutosaveName: NSSearchField.RecentsAutosaveName?

The name under which the search field automatically archives the list of recent search strings.

typealias RecentsAutosaveName

The string that stores the name under which a search field automatically archives a list of recent search strings.

### Getting Search Field Metrics

var cancelButtonBounds: NSRect

The rectangle for the cancel button within the bounds of the search field.

var searchButtonBounds: NSRect

The rectangle for the search button within the bounds of the search field.

var searchTextBounds: NSRect

The rectangle for the search text within the bounds of the search field.

### Deprecated Symbols

var centersPlaceholder: Bool

A Boolean value that determines whether the search field’s components are centered within the control.

Deprecated

func rectForCancelButton(whenCentered: Bool) -> NSRect

The rectangle for the cancel button within the bounds of the search field.

Deprecated

func rectForSearchButton(whenCentered: Bool) -> NSRect

The rectangle for the search button within the bounds of the search field.

Deprecated

func rectForSearchText(whenCentered: Bool) -> NSRect

The rectangle for the search text within the bounds of the field.

Deprecated

## Relationships

### Inherits From

- NSTextField

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityNavigableStaticText
- NSAccessibilityProtocol
- NSAccessibilityStaticText
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTextContent
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

