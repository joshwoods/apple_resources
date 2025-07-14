

- WatchKit
-  WKCrownDelegate 

Protocol

# WKCrownDelegate

A collection of methods you can implement to track the user’s interaction with the digital crown, receiving notifications when the user rotates the crown or when rotation stops.

watchOS 3.0+

``` source
protocol WKCrownDelegate : NSObjectProtocol
```

## Topics

### Receiving Crown Events

func crownDidRotate(WKCrownSequencer?, rotationalDelta: Double)

Called when the user rotates the crown.

func crownDidBecomeIdle(WKCrownSequencer?)

Called when the user stops rotating the crown.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Event handling

class WKCrownSequencer

An object that reports the current state of the digital crown, including its rotational speed when it is in motion.

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

