

- AppKit
-  NSTextAlternatives 

Class

# NSTextAlternatives

A list of alternative strings for a piece of text.

macOS 10.8+

``` source
class NSTextAlternatives
```

## Overview

NSTextAlternatives is an immutable value class that stores a list of alternatives for a piece of text and communicates the user’s selection of an alternative via a notification to your app. To support dictation, for example, you might use NSTextAlternatives to present a list of alternative interpretations for a word or phrase the user speaks. If the user chooses to replace the initial interpretation with an alternative, NSTextAlternatives notifies you of the choice so that you can update the text appropriately.

NSTextAlternatives instances are attached to attributed strings as the value of a text attribute, NSTextAlternativesAttributeName.

## Topics

### Initializing a Text Alternatives Object

init(primaryString: String, alternativeStrings: [String])

Initializes an `NSTextAlternatives` instance.

### Storing Alternative Text Strings

var primaryString: String

The text that was initially chosen as the input string.

var alternativeStrings: [String]

An array of alternative possible interpretations that the user might select.

### Selecting an Alternative String

func noteSelectedAlternativeString(String)

Sent to the `NSTextAlternatives` object by the text view when the user chooses one of the alternative strings.

### Notifications

class let selectedAlternativeStringNotification: NSNotification.Name

Posted when the user selects an alternate string.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Text input

Adopting the system text cursor in custom text views

Incorporate the system text cursor into your custom text UI in AppKit.

class NSTextInputContext

An object that represents the Cocoa text input system.

protocol NSTextInputClient

A set of methods that text views need to implement to interact properly with the text input management system.

protocol NSTextContent

A protocol that describes specific kinds of input content types.

class NSTextInsertionIndicator

A view that represents the insertion indicator in text.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

struct AutomaticModeOptions

Options that affect the automatic display mode.

