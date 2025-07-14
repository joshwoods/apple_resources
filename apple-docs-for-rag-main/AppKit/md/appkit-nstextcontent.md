

- AppKit
-  NSTextContent 

Protocol

# NSTextContent

A protocol that describes specific kinds of input content types.

macOS

``` source
protocol NSTextContent
```

## Topics

### Specifying content type

var contentType: NSTextContentType?

The semantic meaning for a text input area.

**Required**

struct NSTextContentType

Constants that identify the semantic meaning for a text-entry area.

## Relationships

### Conforming Types

- NSComboBox
- NSSearchField
- NSSecureTextField
- NSTextField
- NSTextView
- NSTokenField

## See Also

### Text input

Adopting the system text cursor in custom text views

Incorporate the system text cursor into your custom text UI in AppKit.

class NSTextInputContext

An object that represents the Cocoa text input system.

protocol NSTextInputClient

A set of methods that text views need to implement to interact properly with the text input management system.

class NSTextAlternatives

A list of alternative strings for a piece of text.

class NSTextInsertionIndicator

A view that represents the insertion indicator in text.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

struct AutomaticModeOptions

Options that affect the automatic display mode.

