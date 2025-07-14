

- AppKit
- NSEvent
- NSEvent.EventTypeMask
-  init(type:) 

Initializer

# init(type:)

Returns the event mask for the specified type.

macOS

``` source
init(type: NSEvent.EventType)
```

## Parameters 

`type`  

The event type whose mask you want to get.

## Return Value

The event mask corresponding to the specified type. The returned mask is equivalent to the number 1 left-shifted by `type` bits.

## See Also

### Constants

struct EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

struct ModifierFlags

Flags that represent key states in an event object.

struct Phase

Constants that represent the possible phases during an event phase.

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

