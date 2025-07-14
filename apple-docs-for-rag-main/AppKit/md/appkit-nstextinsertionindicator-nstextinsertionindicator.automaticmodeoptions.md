

- AppKit
- NSTextInsertionIndicator
-  NSTextInsertionIndicator.AutomaticModeOptions 

Structure

# NSTextInsertionIndicator.AutomaticModeOptions

Options that affect the automatic display mode.

macOS 14.0+

``` source
struct AutomaticModeOptions
```

## Topics

### Configuring automatic mode options

static var showEffectsView: NSTextInsertionIndicator.AutomaticModeOptions

Specifies whether a trailing glow displays during dictation.

static var showWhileTracking: NSTextInsertionIndicator.AutomaticModeOptions

Specifies whether the insertion indicator shows during a tracking loop.

### Initializers

init(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

