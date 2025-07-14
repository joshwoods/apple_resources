

- BrowserEngineKit
- BEKeyEntry
-  BEKeyEntry.KeyPressState 

Enumeration

# BEKeyEntry.KeyPressState

An enumeration that represents the possible states of a key-press in a keyboard event.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
enum KeyPressState
```

## Topics

### Key states

case down

The key is down.

case up

The key is up.

### Creating a key-press state

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting information about the keypress

var state: BEKeyEntry.KeyPressState

Type of the event, indicating whether it represents when the key is pressed or released.

var isKeyRepeating: Bool

Represents whether the event is repeating.

var timestamp: TimeInterval

Time at which the key event occurred.

