

- AppKit
- NSWindow
-  nextEvent(matching:until:inMode:dequeue:) 

Instance Method

# nextEvent(matching:until:inMode:dequeue:)

Forwards the message to the global application object.

macOS

``` source
@MainActor
func nextEvent(
    matching mask: NSEvent.EventTypeMask,
    until expiration: Date?,
    inMode mode: RunLoop.Mode,
    dequeue deqFlag: Bool
) -> NSEvent?
```

## Parameters 

`mask`  

The mask that the event to return must match.

`expiration`  

The date until which to wait for events.

`mode`  

The run loop mode to use while waiting for events

`deqFlag`  

true to remove the returned event from the event queue; false to leave the returned event in the queue.

## Return Value

The next event whose mask matches the specified `mask`; otherwise, `nil`.

## See Also

### Related Documentation

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Forwards the message to the global application object.

func postEvent(NSEvent, atStart: Bool)

Forwards the message to the global application object.

func sendEvent(NSEvent)

This action method dispatches mouse and keyboard events the global application object sends to the window.

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

