

- UIKit
- UIControl
-  UIControl.Event 

Structure

# UIControl.Event

Constants describing the types of events possible for controls.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct Event
```

## Mentioned in 

Responding to control-based events using target-action

## Overview

You set up a control so that it sends an action message to a target object by associating both target and action with one or more control events. To do this, send addTarget(_:action:for:) to the control for each target-action pair you want to specify.

## Topics

### Constants

static var touchDown: UIControl.Event

A touch-down event in the control.

static var touchDownRepeat: UIControl.Event

A repeated touch-down event in the control; for this event the value of the UITouch `tapCount` method is greater than one.

static var touchDragInside: UIControl.Event

An event where a finger is dragged inside the bounds of the control.

static var touchDragOutside: UIControl.Event

An event where a finger is dragged just outside the bounds of the control.

static var touchDragEnter: UIControl.Event

An event where a finger is dragged into the bounds of the control.

static var touchDragExit: UIControl.Event

An event where a finger is dragged from within a control to outside its bounds.

static var touchUpInside: UIControl.Event

A touch-up event in the control where the finger is inside the bounds of the control.

static var touchUpOutside: UIControl.Event

A touch-up event in the control where the finger is outside the bounds of the control.

static var touchCancel: UIControl.Event

A system event canceling the current touches for the control.

static var valueChanged: UIControl.Event

A touch dragging or otherwise manipulating a control, causing it to emit a series of different values.

static var menuActionTriggered: UIControl.Event

A menu action has triggered prior to the menu being presented.

static var primaryActionTriggered: UIControl.Event

A semantic action triggered by buttons.

static var editingDidBegin: UIControl.Event

A touch initiating an editing session in a text field by entering its bounds.

static var editingChanged: UIControl.Event

A touch making an editing change in a text field.

static var editingDidEnd: UIControl.Event

A touch ending an editing session in a text field by leaving its bounds.

static var editingDidEndOnExit: UIControl.Event

A touch ending an editing session in a text field.

static var allTouchEvents: UIControl.Event

All touch events.

static var allEditingEvents: UIControl.Event

All editing touches for text fields.

static var applicationReserved: UIControl.Event

A range of control-event values available for app use.

static var systemReserved: UIControl.Event

A range of control-event values reserved for internal framework use.

static var allEvents: UIControl.Event

All events, including system events.

### Initializers

init(rawValue: UInt)

Creates a control event with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

