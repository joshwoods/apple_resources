

- BrowserEngineKit
- BEKeyEntry
-  timestamp 

Instance Property

# timestamp

Time at which the key event occurred.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var timestamp: TimeInterval { get }
```

## Discussion

The time at which the key event occurs.

## See Also

### Getting information about the keypress

var state: BEKeyEntry.KeyPressState

Type of the event, indicating whether it represents when the key is pressed or released.

enum KeyPressState

An enumeration that represents the possible states of a key-press in a keyboard event.

var isKeyRepeating: Bool

Represents whether the event is repeating.

