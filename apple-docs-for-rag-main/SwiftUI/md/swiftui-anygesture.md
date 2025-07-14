

- SwiftUI
-  AnyGesture 

Structure

# AnyGesture

A type-erased gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct AnyGesture
```

## Topics

### Implementing a custom gesture

init&lt;T>(T)

Creates an instance from another gesture.

## Relationships

### Conforms To

- Gesture

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

struct HandActivationBehavior

An activation behavior specific to hand-driven input.

struct HandGestureShortcut

Hand gesture shortcuts describe finger and wrist movements that the user can perform in order to activate a button or toggle.

