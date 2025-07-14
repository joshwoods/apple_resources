

- UIKit
- UIGestureRecognizer
-  modifierFlags 

Instance Property

# modifierFlags

The bit mask of modifier flags in the gesture represented by the gesture recognizer.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var modifierFlags: UIKeyModifierFlags { get }
```

## See Also

### Getting the recognizer’s state and view

var state: UIGestureRecognizer.State

The current state of the gesture recognizer.

enum State

Constants that represent the current state a gesture recognizer is in.

var view: UIView?

The view the gesture recognizer is attached to.

var isEnabled: Bool

A Boolean property that indicates whether the gesture recognizer is enabled.

var buttonMask: UIEvent.ButtonMask

A bit mask of the buttons in the gesture represented by the gesture recognizer.

