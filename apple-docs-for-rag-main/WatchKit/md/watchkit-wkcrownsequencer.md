

- WatchKit
-  WKCrownSequencer 

Class

# WKCrownSequencer

An object that reports the current state of the digital crown, including its rotational speed when it is in motion.

watchOS 3.0+

``` source
class WKCrownSequencer
```

## Overview

Do not create instances of this class yourself. Instead, retrieve a crown sequencer object from the current interface controller’s crownSequencer property. Before the sequencer can receive data, you must call its focus() method. Only one object in your interface can have focus at any given time, so if your interface also contains picker objects or has scrollable scenes, you must coordinate changes in focus accordingly. For example, calling the sequencer’s focus() method causes any picker objects or interface controllers to resign focus. When the user taps on a picker object, the currently active sequencer resigns focus, and the selected picker object gains the focus. Because the crown sequencer is not tied to a specific interface object, you can use it as general input for your app.

Although the crown sequencer object has properties that contain the current state of the crown, it is more common to use a delegate object to receive notifications as the user rotates the crown. For more information on receiving data using a delegate, see WKCrownDelegate.

## Topics

### Getting the Current Crown Status

var rotationsPerSecond: Double

The rotational speed of the crown, measured in rotations per second.

var isIdle: Bool

A Boolean value indicating whether the crown is at rest.

### Accessing the Delegate

var delegate: (any WKCrownDelegate)?

The object you use to monitor changes to the crown state.

### Managing the Focus

func focus()

Begins the delivery of crown events to the current crown sequencer.

func resignFocus()

Ends the delivery of crown events to the current crown sequencer.

### Managing Haptic Feedback

var isHapticFeedbackEnabled: Bool

A Boolean value that determines whether the crown sequencer’s haptic feedback is enabled.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Event handling

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

class WKTapGestureRecognizer

A gesture recognizer that interprets a touch event occurring and ending in approximately the same area on the screen.

