

- UIKit
-  UIEvent 

Class

# UIEvent

An object that describes a single user interaction with your app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIEvent
```

## Mentioned in 

Responding to control-based events using target-action

## Overview

Apps can receive many different types of events, including touch events, motion events, remote-control events, and press events. Touch events are the most common and are delivered to the view in which the touch originally occurred. Motion events are UIKit triggered and are separate from the motion events reported by the Core Motion framework. Remote-control events allow a responder object to receive commands from an external accessory or headset so that it can manage audio and video — for example, playing a video or skipping to the next audio track. Press events represent interactions with a game controller, Apple TV remote, or other device that has physical buttons. You can determine the type of an event using the type and subtype properties.

A touch event object contains the touches (that is, the fingers on the screen) that have some relation to the event. A touch event object may contain one or more touches, and each touch is represented by a UITouch object. When a touch event occurs, the system routes it to the appropriate responder and calls the appropriate method, such as touchesBegan(_:with:). The responder then uses the touches to determine an appropriate course of action.

During a multitouch sequence, UIKit reuses the same UIEvent object when delivering updated touch data to your app. You should never retain an event object or any object returned from an event object. If you need to retain data outside of the responder method you use to process that data, copy that data from the UITouch or UIEvent object to your local data structures.

For more information on how to handle events in your UIKit app, see Event Handling Guide for UIKit Apps.

## Topics

### Getting the touches for an event

var allTouches: Set&lt;UITouch>?

All touches associated with the event.

func touches(for: UIView) -> Set&lt;UITouch>?

Returns the touch objects from the event that belong to the specified given view.

func touches(for: UIWindow) -> Set&lt;UITouch>?

Returns the touch objects from the event that belong to the specified window.

func coalescedTouches(for: UITouch) -> [UITouch]?

Returns all of the touches associated with the specified main touch.

func predictedTouches(for: UITouch) -> [UITouch]?

Returns an array of touches that are predicted to occur for the specified touch.

### Getting event attributes

var timestamp: TimeInterval

The time when the event occurred.

### Getting the event type

var type: UIEvent.EventType

Returns the type of the event.

enum EventType

Constants that specify the general type of an event.

var subtype: UIEvent.EventSubtype

Returns the subtype of the event.

enum EventSubtype

Constants that specify the subtype of the event in relation to its general type.

### Getting the touches for a gesture recognizer

func touches(for: UIGestureRecognizer) -> Set&lt;UITouch>?

Returns the touch objects that are being delivered to the specified gesture recognizer.

### Getting the button mask

var buttonMask: UIEvent.ButtonMask

A bit mask that represents which input-device buttons are pressed for the current event.

struct ButtonMask

Constants that indicate which input-device buttons are pressed.

### Getting the modifier flags

var modifierFlags: UIKeyModifierFlags

The set of modifier keys that are pressed for the current event.

struct UIKeyModifierFlags

Constants that indicate which modifier keys are pressed.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIPressesEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Essentials

Using responders and the responder chain to handle events

Learn how to handle events that propagate through your app.

class UIResponder

An abstract interface for responding to and handling events.

