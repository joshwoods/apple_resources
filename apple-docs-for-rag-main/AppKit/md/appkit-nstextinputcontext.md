

- AppKit
-  NSTextInputContext 

Class

# NSTextInputContext

An object that represents the Cocoa text input system.

macOS 10.6+

``` source
class NSTextInputContext
```

## Overview

The text input system communicates primarily with the client of the activated input context via the NSTextInputClient protocol.

## Topics

### Creating an Input Context

init(client: any NSTextInputClient)

The designated initializer

### Getting the Input Context and Client

class var current: NSTextInputContext?

Returns the current, activated, text input context object.

var client: any NSTextInputClient

The owner of this input context. (read-only)

### Configuring the Input Context

var acceptsGlyphInfo: Bool

A Boolean value that indicates whether the client handles `NSGlyphInfoAttributeName` or not.

var allowedInputSourceLocales: [String]?

The set of keyboard input source locales allowed when this input context is active.

### Activating the Input Context

func activate()

Activates the receiver.

func deactivate()

Deactivates the receiver.

### Handling Input Sources

func handleEvent(NSEvent) -> Bool

Tells the Cocoa text input system to handle mouse or key events.

func discardMarkedText()

Tells the Cocoa text input system to discard the current conversion session.

func invalidateCharacterCoordinates()

Notifies the Cocoa text input system that the position information previously queried via methods like `firstRectForCharacterRange:actualRange:` needs to be updated.

var keyboardInputSources: [NSTextInputSourceIdentifier]?

The array of keyboard text input source identifier strings available to the receiver. (read-only)

var selectedKeyboardInputSource: NSTextInputSourceIdentifier?

The identifier string for the selected keyboard text input source.

class func localizedName(forInputSource: NSTextInputSourceIdentifier) -> String?

Returns the display name for the given text input source identifier.

typealias NSTextInputSourceIdentifier

### Notifications

class let keyboardSelectionDidChangeNotification: NSNotification.Name

Posted after the selected text input source changes.

### Instance Methods

func textInputClientDidEndScrollingOrZooming()

func textInputClientWillStartScrollingOrZooming()

func textInputClientDidScroll()

func textInputClientDidUpdateSelection()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Text input

Adopting the system text cursor in custom text views

Incorporate the system text cursor into your custom text UI in AppKit.

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

struct AutomaticModeOptions

Options that affect the automatic display mode.

