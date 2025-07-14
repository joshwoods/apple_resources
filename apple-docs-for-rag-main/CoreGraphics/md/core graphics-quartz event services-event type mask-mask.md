

- Core Graphics
- Quartz Event Services
-  Event Type Mask 

API Collection

# Event Type Mask

Specifies an event mask that represents all event types.

## Overview

This constant is typically used with the functions tapCreate(tap:place:options:eventsOfInterest:callback:userInfo:) and tapCreateForPSN(processSerialNumber:place:options:eventsOfInterest:callback:userInfo:) to register an event tap that observes all input events.

## See Also

### Constants

enum CGEventField

Constants used as keys to access specialized fields in low-level events.

struct CGEventFilterMask

Specify masks for classes of low-level events that can be filtered during event suppression states.

struct CGEventFlags

Constants that indicate the modifier key state at the time an event is created, as well as other event-related states.

enum CGEventSourceStateID

Constants that specify the possible source states of an event source.

Event Source Token

Specifies any input event type.

enum CGEventSuppressionState

Specify the event suppression states that can occur after posting an event.

enum CGEventTapLocation

Constants that specify possible tapping points for events.

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

enum CGEventTapPlacement

Constants that specify where a new event tap is inserted into the list of active event taps.

enum CGEventType

Constants that specify the different types of input events.

enum CGMouseButton

Constants that specify buttons on a one, two, or three-button mouse.

enum CGEventMouseSubtype

Constants used with the CGEventField.mouseEventSubtype event field.

enum CGScrollEventUnit

Constants that specify the unit of measurement for a scrolling event.

