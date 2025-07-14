

- AppKit
-  NSTextInsertionIndicator 

Class

# NSTextInsertionIndicator

A view that represents the insertion indicator in text.

macOS 14.0+

``` source
@MainActor
class NSTextInsertionIndicator
```

## Mentioned in 

Adopting the system text cursor in custom text views

## Overview

NSTextView and NSTextField both use NSTextInsertionIndicator to display the insertion indicator. You can use this indicator if you have your own text engine or need to display an indicator elsewhere.

To use the indicator, instantiate an NSTextInsertionIndicator, then add the view to your view hierarchy. Set the indicator view’s frame to where you want to display a text insertion indicator. The indicator has the same height as the indicator view’s frame, and centers horizontally within the indicator view’s frame.

The NSTextInsertionIndicator.DisplayMode specifies whether the indicator hides, remains visible, or blinks (automatic).

When set to NSTextInsertionIndicator.DisplayMode.automatic, the indicator stops blinking when you set the frame. The indicator starts blinking when the frame doesn’t change for a period of time. When the user dictates, the indicator displays a trailing glow when it is moved.

Set the NSTextInsertionIndicator.DisplayMode to NSTextInsertionIndicator.DisplayMode.automatic when your custom view becomes the first responder. When your custom view resigns first responder, set the displayMode to NSTextInsertionIndicator.DisplayMode.hidden to indicate that key events aren’t sent to your view.

By default the indicator’s color is textInsertionPointColor. You can set a different color.

## Topics

### Configuring indicators

var color: NSColor!

The color of this indicator.

var effectsViewInserter: ((NSView) -> Void)?

An optional closure the system calls during dictation.

### Setting the display mode

var displayMode: NSTextInsertionIndicator.DisplayMode

A value that describes the display mode of an indicator.

var automaticModeOptions: NSTextInsertionIndicator.AutomaticModeOptions

Options that affect the automatic display mode.

struct AutomaticModeOptions

Options that affect the automatic display mode.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

## Relationships

### Inherits From

- NSView

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
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

struct AutomaticModeOptions

Options that affect the automatic display mode.

