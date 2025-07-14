

- BrowserEngineKit
-  BEKeyEntry 

Class

# BEKeyEntry

A class that represents a keyboard event in the text system.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
class BEKeyEntry
```

## Topics

### Identifying the key

var key: UIKey

Data about the key that was pressed

### Getting information about the keypress

var state: BEKeyEntry.KeyPressState

Type of the event, indicating whether it represents when the key is pressed or released.

enum KeyPressState

An enumeration that represents the possible states of a key-press in a keyboard event.

var isKeyRepeating: Bool

Represents whether the event is repeating.

var timestamp: TimeInterval

Time at which the key event occurred.

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

### Keyboard input

class BEKeyEntryContext

A class that describes a key event and the text document with which the event is associated.

enum BEKeyModifierFlags

An enumeration that records the state of the shift-modifier keys.

