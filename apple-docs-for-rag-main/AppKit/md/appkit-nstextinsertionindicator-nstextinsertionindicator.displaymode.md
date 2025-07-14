

- AppKit
- NSTextInsertionIndicator
-  NSTextInsertionIndicator.DisplayMode 

Enumeration

# NSTextInsertionIndicator.DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

macOS 14.0+

``` source
enum DisplayMode
```

## Topics

### Defining the display mode

case automatic

case hidden

case visible

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

protocol NSTextContent

A protocol that describes specific kinds of input content types.

class NSTextInsertionIndicator

A view that represents the insertion indicator in text.

struct AutomaticModeOptions

Options that affect the automatic display mode.

