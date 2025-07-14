

- BrowserEngineKit
- BEKeyEntry
-  state 

Instance Property

# state

Type of the event, indicating whether it represents when the key is pressed or released.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var state: BEKeyEntry.KeyPressState { get }
```

## Discussion

Whether the key is pressed or released.

## See Also

### Getting information about the keypress

enum KeyPressState

An enumeration that represents the possible states of a key-press in a keyboard event.

var isKeyRepeating: Bool

Represents whether the event is repeating.

var timestamp: TimeInterval

Time at which the key event occurred.

