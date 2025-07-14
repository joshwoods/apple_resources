

- WatchKit
-  WKGestureRecognizer 

Class

# WKGestureRecognizer

The base class for all other gesture recognizer classes.

watchOS 3.0+

``` source
class WKGestureRecognizer
```

## Overview

Gesture recognizers simplify the event-handling process by tracking touch events for you and calling your custom code when those events match a specific pattern. Gesture recognizers report the results of their tracking to an action method that you define.

You do not subclass WKGestureRecognizer or create instances of it directly. Instead, you add concrete gesture recognizer objects to your Watch app’s storyboard file and connect that gesture recognizer to your custom action method. At runtime, you use the methods of this class to get and set the state of your gesture recognizer. The concrete gesture recognizer classes are as follows:

- WKLongPressGestureRecognizer

- WKPanGestureRecognizer

- WKSwipeGestureRecognizer

- WKTapGestureRecognizer

### Executing Code in Response to a Gesture

A gesture recognizer has an associated action method that it calls during the recognition process to report on its progress. You define the action method in your interface controller and connect it to the gesture recognizer in Interface Builder. Action methods must conform to one of the following signatures:

- Swift
- Objective-C

```
@IBAction func handleGesture()
@IBAction func handleGesture(gestureRecognizer : WKGestureRecognizer)
```

```
```

The gesture recognizer calls your action method whenever the value in the state property changes in a significant way. All gesture recognizers start out in the WKGestureRecognizerState.possible state and move to other states as appropriate based on the type of gesture. Gesture recognizers do not call your action method for every state change. For information about when the action method is called, see the constant descriptions of the WKGestureRecognizerState type.

watchOS supports two broad categories of gesture recognizers: continuous gesture recognizers and discrete gesture recognizer.

#### Continuous Gesture Recognizers

Continuous gesture recognizers—for example, pan or long touch recognizers—track the user’s gesture and call the action method multiple times during a single gesture. They typically call the action method once when the gesture begins, one or more times as the gesture progresses, and once when the gesture either ends or is canceled. In your action method, use the gesture recognizer’s state property to perform appropriate tasks based on the current state. For example:

- WKGestureRecognizerState.began. Alter the user interface’s appearance to indicate that a gesture has begun.

- WKGestureRecognizerState.changed. Update the user interface based on the current touch location.

- WKGestureRecognizerState.ended. Return to the normal user interface appearance, indicating that the gesture has ended. Keep any updates.

- WKGestureRecognizerState.cancelled. Return to the normal user interface appearance, indicating that the gesture has ended. Discard any updates.

#### Discrete Gesture Recognizers

Discrete gesture recognizers—for example, tap or swipe recognizers—only trigger a single event as soon as the gesture is recognized. For example, discrete recognizers call their action method when they enter the WKGestureRecognizerState.recognized state. If they enter the WKGestureRecognizerState.failed state, they fail silently.

### Interface Builder Attributes

Xcode lets you configure information about your gesture recognizer in your storyboard file. The following table lists the attributes you can configure in your storyboard and their meaning.

| Attribute | Description |
|----|----|
| State | A checkbox indicating whether the gesture recognizer is enabled. You can also configure this value programmatically using the isEnabled property. |
| Behavior | Checkboxes indicating additional gesture recognizer behaviors. Use these options to specify how the gesture recognizer responds to touch events. |
| Must Fail First | Gesture recognizers that must fail before the current one can succeed. Drag from this option to the gesture recognizers in your storyboard file. |

## Topics

### Getting the Touch Information

func locationInObject() -> CGPoint

Returns the point computed as the current position of the touch event.

func objectBounds() -> CGRect

Returns the dimensions of the interface object (measured in points) associated with the gesture recognizer.

### Getting the Gesture Recognizer’s State

var state: WKGestureRecognizerState

The current state of the gesture recognizer.

var isEnabled: Bool

A Boolean value indicating whether the gesture recognizer is enabled.

### Constants

enum WKGestureRecognizerState

Constants describing the possible states of a gesture recognizer.

## Relationships

### Inherits From

- NSObject

### Inherited By

- WKLongPressGestureRecognizer
- WKPanGestureRecognizer
- WKSwipeGestureRecognizer
- WKTapGestureRecognizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Event handling

class WKCrownSequencer

An object that reports the current state of the digital crown, including its rotational speed when it is in motion.

protocol WKCrownDelegate

A collection of methods you can implement to track the user’s interaction with the digital crown, receiving notifications when the user rotates the crown or when rotation stops.

class WKLongPressGestureRecognizer

A gesture recognizer that interprets a touch event that occurs in the same relative area for an extended period of time.

class WKPanGestureRecognizer

A gesture recognizer that interprets a touch event that moves around the screen.

class WKSwipeGestureRecognizer

A gesture recognizer that interprets swiping gestures in one or more directions.

class WKTapGestureRecognizer

A gesture recognizer that interprets a touch event occurring and ending in approximately the same area on the screen.

