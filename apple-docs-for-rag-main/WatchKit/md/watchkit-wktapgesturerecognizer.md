

- WatchKit
-  WKTapGestureRecognizer 

Class

# WKTapGestureRecognizer

A gesture recognizer that interprets a touch event occurring and ending in approximately the same area on the screen.

watchOS 3.0+

``` source
class WKTapGestureRecognizer
```

## Overview

The tap gesture recognizer can report when a single tap happens or when multiple taps happen.

You do not create instances of this class programmatically. Instead, add a tap gesture recognizer to your Watch appʼs storyboard file, dropping it onto a specific interface object. The gesture recognizer tracks touches that occur within the bounds of that interface object and reports to an action method you define on the parent interface controller. For information on defining your action method and connecting it to your gesture recognizer, see WKGestureRecognizer.

### State Changes for a Tap Gesture

A tap gesture recognizer tracks discrete events, and therefore has a limited number of state changes. Each tap in a tap gesture comprises the user touching the screen and then lifting the finger off the screen in about the same location and within a preset amount of time. Gesture recognition occurs when the user performs the specified number of taps. The state transition sequences for a tap gesture are as follows:

The gesture recognizer calls its action method when it enters the WKGestureRecognizerState.recognized state. You can determine the location of the tap by calling its locationInObject() method. For more information on implementing discrete gesture recognizers, see WKGestureRecognizer.

### Interface Builder Attributes

Xcode lets you configure information about your gesture recognizer in your storyboard file. The following table lists the attributes you can configure in your storyboard and their meanings.

| Attribute | Description |
|----|----|
| Taps | The number of taps necessary to complete the gesture. You can set this value using the numberOfTapsRequired property. |

The WKGestureRecognizer parent class also defines attributes that you can configure for your gesture recognizer. For information about those attributes, see WKGestureRecognizer.

## Topics

### Configuring the Gesture

var numberOfTapsRequired: Int

The number of taps necessary for gesture recognition.

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

class WKPanGestureRecognizer

A gesture recognizer that interprets a touch event that moves around the screen.

class WKSwipeGestureRecognizer

A gesture recognizer that interprets swiping gestures in one or more directions.

