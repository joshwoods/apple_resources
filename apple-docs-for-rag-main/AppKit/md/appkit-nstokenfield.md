

- AppKit
-  NSTokenField 

Class

# NSTokenField

A text field that converts text into visually distinct tokens.

macOS

``` source
@MainActor
class NSTokenField
```

## Overview

Use a token field when you want typed text to be transformed into “tokens”, which are visually distinct elements in the text field interface. For example, you might use a token field in a mail app to display email addresses for individual users. The distinct appearance of tokens makes them easy for users to distinguish from surrounding text.

`NSTokenField` uses an NSTokenFieldCell to implement much of the control’s functionality. `NSTokenField` provides cover methods for most methods of `NSTokenFieldCell`, which invoke the corresponding cell method.

Notes

In OS X v10.4 and earlier, represented objects associated with token fields had to conform to NSCoding. Starting with OS X v10.5, they no longer need to.

In OS X v10.4, `NSTokenField` trims whitespace around tokens but it does not trim whitespace in macOS versions 10.5.0 and 10.5.1. In OS X v10.5.2, you get whitespace-trimming behavior by either linking against the v10.4 binary or linking against the v10.5 binary and *not* implementing the tokenField(_:representedObjectForEditing:) method. If you do not want the whitespace-trimming behavior, link against the v10.5 binary and implement this method, returning the editing string if you have no represented object.

## Topics

### Configuring the Token Style

var tokenStyle: NSTokenField.TokenStyle

The token style of the receiver.

### Configuring the Tokenizing Character Set

var tokenizingCharacterSet: CharacterSet!

The recevier’s tokenizing character set to `characterSet`.

class var defaultTokenizingCharacterSet: CharacterSet

Returns the default tokenizing character set.

### Configuring the Completion Delay

var completionDelay: TimeInterval

The receiver’s completion delay.

class var defaultCompletionDelay: TimeInterval

Returns the default completion delay.

### Getting and Setting the Delegate

var delegate: (any NSTokenFieldDelegate)?

Returns the token field’s delegate.

### Enumerations

enum TokenStyle

The NSTokenStyle constants define how tokens are displayed and editable in the `NSTokenFieldCell`. These values are used by tokenStyle and the delegate method tokenFieldCell(_:styleForRepresentedObject:).

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

