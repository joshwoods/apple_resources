

- AppKit
- NSWindow
-  sendEvent(\_:) 

Instance Method

# sendEvent(\_:)

This action method dispatches mouse and keyboard events the global application object sends to the window.

macOS

``` source
@MainActor
func sendEvent(_ event: NSEvent)
```

## Parameters 

`event`  

The mouse or keyboard event to process.

## Discussion

Never invoke this method directly. A right mouse-down event in a window of an inactive application isn’t delivered to the corresponding `NSWindow` object. Instead, a sendEvent(_:) message with a window number of `0` delivers it to the NSApplication object.

## See Also

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Forwards the message to the global application object.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Forwards the message to the global application object.

func postEvent(NSEvent, atStart: Bool)

Forwards the message to the global application object.

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

