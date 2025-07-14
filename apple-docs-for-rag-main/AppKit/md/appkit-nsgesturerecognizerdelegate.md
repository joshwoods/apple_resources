

- AppKit
-  NSGestureRecognizerDelegate 

Protocol

# NSGestureRecognizerDelegate

A set of methods for fine-tuning a gesture recognizer’s behavior.

macOS

``` source
protocol NSGestureRecognizerDelegate : NSObjectProtocol
```

## Overview

Use the methods in this protocol to establish dynamic dependencies between gesture recognizers and to prevent a single gesture recognizer from acting at all.

## Topics

### Regulating Gesture Recognition

func gestureRecognizer(NSGestureRecognizer, shouldAttemptToRecognizeWith: NSEvent) -> Bool

Asks the delegate if a gesture recognizer should attempt to recognize gestures for a particular event.

func gestureRecognizerShouldBegin(NSGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should transition out of the Possible (`NSGestureRecognizerStatePossible`) state.

### Controlling Simultaneous Gesture Recognition

func gestureRecognizer(NSGestureRecognizer, shouldRecognizeSimultaneouslyWith: NSGestureRecognizer) -> Bool

Asks the delegate if two gesture recognizers should be allowed to recognize their gestures simultaneously.

### Setting Up Failure Requirements

func gestureRecognizer(NSGestureRecognizer, shouldRequireFailureOf: NSGestureRecognizer) -> Bool

Asks the delegate if the current gesture recognizer must wait to recognize its gesture until the specified gesture recognizer fails.

func gestureRecognizer(NSGestureRecognizer, shouldBeRequiredToFailBy: NSGestureRecognizer) -> Bool

Asks the delegate if the current gesture recognizer must fail before another gesture recognizer is allowed to recognize its gesture.

### Instance Methods

func gestureRecognizer(NSGestureRecognizer, shouldReceive: NSTouch) -> Bool

Called, for a new touch, before the system calls the `touchesBegan:withEvent:` method on the gesture recognizer. Return `NO` to prevent the gesture recognizer from seeing this touch.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Custom Gestures

class NSGestureRecognizer

An object that monitors events and calls its action method when a predefined sequence of events occur.

