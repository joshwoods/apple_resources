

- AppKit
- NSWindow
-  discardEvents(matching:before:) 

Instance Method

# discardEvents(matching:before:)

Forwards the message to the global application object.

macOS

``` source
@MainActor
func discardEvents(
    matching mask: NSEvent.EventTypeMask,
    before lastEvent: NSEvent?
)
```

## Parameters 

`mask`  

The mask of the events to discard.

`lastEvent`  

The event up to which queued events are discarded from the queue.

## See Also

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Forwards the message to the global application object.

func postEvent(NSEvent, atStart: Bool)

Forwards the message to the global application object.

func sendEvent(NSEvent)

This action method dispatches mouse and keyboard events the global application object sends to the window.

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

