

- SwiftUI
-  Gesture 

Protocol

# Gesture

An instance that matches a sequence of events to a gesture, and returns a stream of values for each of its states.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol Gesture
```

## Overview

Create custom gestures by declaring types that conform to the `Gesture` protocol.

## Topics

### Implementing a custom gesture

var body: Self.Body

The content and behavior of the gesture.

**Required**

associatedtype Body : Gesture

The type of gesture representing the body of `Self`.

**Required**

### Performing the gesture

func updating&lt;State>(GestureState&lt;State>, body: (Self.Value, inout State, inout Transaction) -> Void) -> GestureStateGesture&lt;Self, State>

Updates the provided gesture state property as the gesture’s value changes.

func onChanged((Self.Value) -> Void) -> _ChangedGesture&lt;Self>

Adds an action to perform when the gesture’s value changes.

func onEnded((Self.Value) -> Void) -> _EndedGesture&lt;Self>

Adds an action to perform when the gesture ends.

associatedtype Value

The type representing the gesture’s value.

**Required**

### Composing gestures

func simultaneously&lt;Other>(with: Other) -> SimultaneousGesture&lt;Self, Other>

Combines a gesture with another gesture to create a new gesture that recognizes both gestures at the same time.

func sequenced&lt;Other>(before: Other) -> SequenceGesture&lt;Self, Other>

Sequences a gesture with another one to create a new gesture, which results in the second gesture only receiving events after the first gesture succeeds.

func exclusively&lt;Other>(before: Other) -> ExclusiveGesture&lt;Self, Other>

Combines two gestures exclusively to create a new gesture where only one gesture succeeds, giving precedence to the first gesture.

### Adding modifier keys to a gesture

func modifiers(EventModifiers) -> _ModifiersGesture&lt;Self>

Combines a gesture with keyboard modifiers.

### Transforming a gesture

func map&lt;T>((Self.Value) -> T) -> _MapGesture&lt;Self, T>

Returns a gesture that uses the given closure to map over this gesture’s value.

### Customizing gesture activation

func handActivationBehavior(HandActivationBehavior) -> some Gesture&lt;Self.Value> 

Customizes the activation behavior for a gesture when driven by hand or hand-like input.

### Using a gesture with a RealityKit entity

func targetedToAnyEntity() -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity.

func targetedToEntity(Entity) -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity or a descendant of entity.

func targetedToEntity(where: QueryPredicate&lt;Entity>) -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity that can be found in the results of the query.

## Relationships

### Conforming Types

- AnyGesture
- DragGesture
- ExclusiveGesture
- GestureStateGesture
- LongPressGesture
- MagnificationGesture
- MagnifyGesture
- RotateGesture
- RotateGesture3D
- RotationGesture
- SequenceGesture
- SimultaneousGesture
- SpatialEventGesture
- SpatialTapGesture
- TapGesture
- WindowDragGesture

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

struct AnyGesture

A type-erased gesture.

struct HandActivationBehavior

An activation behavior specific to hand-driven input.

struct HandGestureShortcut

Hand gesture shortcuts describe finger and wrist movements that the user can perform in order to activate a button or toggle.

