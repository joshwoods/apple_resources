

- BrowserEngineKit
-  BEKeyModifierFlags 

Enumeration

# BEKeyModifierFlags

An enumeration that records the state of the shift-modifier keys.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
enum BEKeyModifierFlags
```

## Topics

### Getting caps-shift information

case capsLock

The caps lock is engaged.

case shift

The shift key is pressed down.

case none

There aren’t any active key modifiers.

### Initializing the flags

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

### Keyboard input

class BEKeyEntry

A class that represents a keyboard event in the text system.

class BEKeyEntryContext

A class that describes a key event and the text document with which the event is associated.

