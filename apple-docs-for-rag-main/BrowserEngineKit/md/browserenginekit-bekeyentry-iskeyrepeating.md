

- BrowserEngineKit
- BEKeyEntry
-  isKeyRepeating 

Instance Property

# isKeyRepeating

Represents whether the event is repeating.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var isKeyRepeating: Bool { get }
```

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

For example, a continued press and hold on a key may result in its repeated insertion.

A Boolean value that indicates whether the person is holding the key down to repeat the key event.

## See Also

### Getting information about the keypress

var state: BEKeyEntry.KeyPressState

Type of the event, indicating whether it represents when the key is pressed or released.

enum KeyPressState

An enumeration that represents the possible states of a key-press in a keyboard event.

var timestamp: TimeInterval

Time at which the key event occurred.

