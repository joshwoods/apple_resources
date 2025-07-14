

- UIKit
- UIPress
-  key 

Instance Property

# key

The key pressed or released on a physical keyboard.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var key: UIKey? { get }
```

## Mentioned in 

Handling key presses made on a physical keyboard

## Discussion

This property is `nil` when the press event isn’t from a keyboard; for example, a button press on an Apple TV remote.

## See Also

### Getting press attributes

var type: UIPress.PressType

The type of the specified press.

var phase: UIPress.Phase

The current press phase of the object.

var timestamp: TimeInterval

The time when the press occurred or when it was last mutated.

