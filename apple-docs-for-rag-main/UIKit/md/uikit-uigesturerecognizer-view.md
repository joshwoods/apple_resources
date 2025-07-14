

- UIKit
- UIGestureRecognizer
-  view 

Instance Property

# view

The view the gesture recognizer is attached to.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var view: UIView? { get }
```

## Discussion

You attach (or add) a gesture recognizer to a `UIView` object using the addGestureRecognizer(_:) method.

## See Also

### Getting the recognizer’s state and view

var state: UIGestureRecognizer.State

The current state of the gesture recognizer.

enum State

Constants that represent the current state a gesture recognizer is in.

var isEnabled: Bool

A Boolean property that indicates whether the gesture recognizer is enabled.

var buttonMask: UIEvent.ButtonMask

A bit mask of the buttons in the gesture represented by the gesture recognizer.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier flags in the gesture represented by the gesture recognizer.

