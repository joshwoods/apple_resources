

- UIKit
- UIGestureRecognizer
-  UIGestureRecognizer.State 

Enumeration

# UIGestureRecognizer.State

Constants that represent the current state a gesture recognizer is in.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum State
```

## Overview

Gesture recognizers recognize a discrete event such as a tap or a swipe but don’t report changes within the gesture. In other words, discrete gestures don’t transition through the Began and Changed states and they can’t fail or be canceled.

## Topics

### Constants

case possible

The gesture recognizer hasn’t yet recognized its gesture, but may be evaluating touch events.

case began

The gesture recognizer has received touch objects recognized as a continuous gesture.

case changed

The gesture recognizer has received touches recognized as a change to a continuous gesture.

case ended

The gesture recognizer has received touches recognized as the end of a continuous gesture.

case cancelled

The gesture recognizer has received touches resulting in the cancellation of a continuous gesture.

case failed

The gesture recognizer has received a multi-touch sequence that it can’t recognize as its gesture.

static var recognized: UIGestureRecognizer.State

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the recognizer’s state and view

var state: UIGestureRecognizer.State

The current state of the gesture recognizer.

var view: UIView?

The view the gesture recognizer is attached to.

var isEnabled: Bool

A Boolean property that indicates whether the gesture recognizer is enabled.

var buttonMask: UIEvent.ButtonMask

A bit mask of the buttons in the gesture represented by the gesture recognizer.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier flags in the gesture represented by the gesture recognizer.

