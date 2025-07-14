

- AppKit
- NSWindow
-  postEvent(\_:atStart:) 

Instance Method

# postEvent(\_:atStart:)

Forwards the message to the global application object.

macOS

``` source
@MainActor
func postEvent(
    _ event: NSEvent,
    atStart flag: Bool
)
```

## Parameters 

`event`  

The event to add to the window’s event queue.

`flag`  

true to place the event in the front of the queue; false to place it in the back.

## See Also

### Related Documentation

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Forwards the message to the global application object.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Forwards the message to the global application object.

func sendEvent(NSEvent)

This action method dispatches mouse and keyboard events the global application object sends to the window.

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

