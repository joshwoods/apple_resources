

- SwiftUI
-  HandActivationBehavior 

Structure

# HandActivationBehavior

An activation behavior specific to hand-driven input.

visionOS 1.0+

``` source
struct HandActivationBehavior
```

## Overview

Hand activation behavior determines what hand input modes activate a gesture.

## Topics

### Getting the behaviors

static let automatic: HandActivationBehavior

The default activation behavior, including direct touch, direct pinch, and indirect pinch.

static let pinch: HandActivationBehavior

Activation that requires a pinched hand.

## Relationships

### Conforms To

- Equatable

## See Also

### Defining custom gestures

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func handGestureShortcut(HandGestureShortcut, isEnabled: Bool) -> some View

Assigns a hand gesture shortcut to the modified control.

func defersSystemGestures(on: Edge.Set) -> some View

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

protocol Gesture

An instance that matches a sequence of events to a gesture, and returns a stream of values for each of its states.

struct AnyGesture

A type-erased gesture.

struct HandGestureShortcut

Hand gesture shortcuts describe finger and wrist movements that the user can perform in order to activate a button or toggle.

