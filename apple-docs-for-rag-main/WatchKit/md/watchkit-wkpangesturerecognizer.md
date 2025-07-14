

- WatchKit
-  WKPanGestureRecognizer 

Class

# WKPanGestureRecognizer

A gesture recognizer that interprets a touch event that moves around the screen.

watchOS 3.0+

``` source
class WKPanGestureRecognizer
```

## Overview

In watchOS, a pan gesture must track exactly one touch event, but that touch event may move freely. Pan gestures are often used to drag content around a given area.

You do not create instances of this class programmatically. Instead, add a pan gesture recognizer to your Watch app’s storyboard file, dropping it onto a specific interface object. Touches occurring within the bounds of that interface object are tracked by the gesture recognizer and reported to an action method you define on the parent interface controller. For information on defining your action method and connecting it to your gesture recognizer, see WKGestureRecognizer.

### State Changes for a Pan Gesture

A pan gesture recognizer tracks touch events continuously, and therefore has many potential state changes. A pan gesture does not transition to the Began state until after the touch event starts moving. After that, it may transition to the Changed state, to the Ended, state, to the Failed state, or to the Cancelled state. The two most common state transition sequences are as follows:

- Possible —\> Began —\> \[Changed…\] —\> Ended

- Possible —\> Began —\> \[Changed…\] —\> Failed

The Changed state is optional and may occur multiple times before the Ended, Failed, or Cancelled state is reached. The gesture recognizer calls its action method at each state transition. For more information on implementing continuous gesture recognizers, see WKGestureRecognizer.

### Interface Builder Attributes

Xcode lets you configure information about your gesture recognizer in your storyboard file. A pan gesture recognizer defines no attributes of its own, but you can configure attributes of the WKGestureRecognizer parent class. For information about those attributes, see WKGestureRecognizer.

## Topics

### Tracking the Location and Velocity of the Gesture

func translationInObject() -> CGPoint

The amount of translation for the pan gesture in the current object.

func velocityInObject() -> CGPoint

The velocity of the pan gesture in the current object.

## Relationships

### Inherits From

- WKGestureRecognizer

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

class WKGestureRecognizer

The base class for all other gesture recognizer classes.

class WKLongPressGestureRecognizer

A gesture recognizer that interprets a touch event that occurs in the same relative area for an extended period of time.

class WKSwipeGestureRecognizer

A gesture recognizer that interprets swiping gestures in one or more directions.

class WKTapGestureRecognizer

A gesture recognizer that interprets a touch event occurring and ending in approximately the same area on the screen.

