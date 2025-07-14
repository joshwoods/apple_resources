

- AppKit
-  NSTokenFieldCell 

Class

# NSTokenFieldCell

A text field cell subclass that enables tokenized editing of an array of objects.

macOS

``` source
@MainActor
class NSTokenFieldCell
```

## Overview

NSTokenFieldCell is a subclass of NSTextFieldCell that provides tokenized editing of an array of objects similar to the address field in the Mail app. The objects may be strings or objects that can be represented as strings. A single token field cell can be presented in an NSTokenField control.

## Topics

### Managing the Token Style

var tokenStyle: NSTokenField.TokenStyle

The token style of the receiver.

### Managing the Tokenizing Character Set

class var defaultTokenizingCharacterSet: CharacterSet

Returns the default tokenizing character set.

var tokenizingCharacterSet: CharacterSet!

The receiver’s tokenizing character set to a given character set.

### Configuring the Completion Delay

var completionDelay: TimeInterval

The receiver’s completion delay to a given delay.

class var defaultCompletionDelay: TimeInterval

Returns the default completion delay.

### Managing the Delegate

var delegate: (any NSTokenFieldCellDelegate)?

The receiver’s delegate.

### Constants

enum TokenStyle

The NSTokenStyle constants define how tokens are displayed and editable in the `NSTokenFieldCell`. These values are used by tokenStyle and the delegate method tokenFieldCell(_:styleForRepresentedObject:).

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

## See Also

### Cell

protocol NSTokenFieldCellDelegate

A set of optional methods implemented by delegates of NSTokenFieldCell objects to work with tokenized strings.

