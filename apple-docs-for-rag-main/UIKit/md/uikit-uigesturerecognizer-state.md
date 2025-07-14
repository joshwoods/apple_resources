

- UIKit
- UIGestureRecognizer
-  state 

Instance Property

# state

The current state of the gesture recognizer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var state: UIGestureRecognizer.State { get set }
```

## Mentioned in 

About the Gesture Recognizer State Machine

Handling tap gestures

## Discussion

The possible states a gesture recognizer can be in are represented by the constants of type UIGestureRecognizer.State. Some of these states aren’t applicable to discrete gestures. The read-only version of the state property is intended for clients of a gesture-recognizer class and not subclasses.

### Special considerations

Subclasses of UIGestureRecognizer must use a read-write version of the state property. They get this redeclaration when they import the `UIGestureRecognizerSubclass.h` header file (for Objective-C) or the `UIKit.UIGestureRecognizerSubclass` module (for Swift):

```
@property(nonatomic,readwrite) UIGestureRecognizerState state;
```

Recognizers for discrete gestures transition from UIGestureRecognizer.State.possible to UIGestureRecognizer.State.failed or recognized. Recognizers for continuous gesture transition from UIGestureRecognizer.State.possible to these phases in the given order: UIGestureRecognizer.State.began, UIGestureRecognizer.State.changed, and UIGestureRecognizer.State.ended. If, however, they receive a cancellation touch, they should transition to UIGestureRecognizer.State.cancelled. If recognizers for continuous gestures can’t interpret a multi-touch sequence as their gesture, they transition to UIGestureRecognizer.State.failed.

## See Also

### Getting the recognizer’s state and view

enum State

Constants that represent the current state a gesture recognizer is in.

var view: UIView?

The view the gesture recognizer is attached to.

var isEnabled: Bool

A Boolean property that indicates whether the gesture recognizer is enabled.

var buttonMask: UIEvent.ButtonMask

A bit mask of the buttons in the gesture represented by the gesture recognizer.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier flags in the gesture represented by the gesture recognizer.

