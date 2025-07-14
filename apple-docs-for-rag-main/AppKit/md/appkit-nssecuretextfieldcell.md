

- AppKit
-  NSSecureTextFieldCell 

Class

# NSSecureTextFieldCell

A text field whose value is hidden from the user.

macOS

``` source
@MainActor
class NSSecureTextFieldCell
```

## Overview

NSSecureTextFieldCell works with NSSecureTextField and overrides the general cell use of the field editor to provide its own field editor, which doesn’t display text or allow the user to cut or copy its value.

## Topics

### Working with character echo

var echosBullets: Bool

A Boolean that indicates whether the receiver echoes a bullet character rather than each character typed.

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

class NSTextFieldCell

An object that enhances the text display capabilities of a cell.

