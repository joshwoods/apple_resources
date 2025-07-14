

- UIKit
- UIGestureRecognizer
-  isEnabled 

Instance Property

# isEnabled

A Boolean property that indicates whether the gesture recognizer is enabled.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

Disables a gesture recognizers so it does not receive touches. The default value is true. If you change this property to false while a gesture recognizer is currently recognizing a gesture, the gesture recognizer transitions to a cancelled state.

## See Also

### Getting the recognizer’s state and view

var state: UIGestureRecognizer.State

The current state of the gesture recognizer.

enum State

Constants that represent the current state a gesture recognizer is in.

var view: UIView?

The view the gesture recognizer is attached to.

var buttonMask: UIEvent.ButtonMask

A bit mask of the buttons in the gesture represented by the gesture recognizer.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier flags in the gesture represented by the gesture recognizer.

