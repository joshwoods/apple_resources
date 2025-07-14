

- AppKit
- NSWindow
-  currentEvent 

Instance Property

# currentEvent

The event currently being processed by the application.

macOS

``` source
@MainActor
var currentEvent: NSEvent? { get }
```

## Discussion

The value of this property is given by calling by invoking the NSApplication method currentEvent.

## See Also

### Handling Events

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Forwards the message to the global application object.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Forwards the message to the global application object.

func postEvent(NSEvent, atStart: Bool)

Forwards the message to the global application object.

func sendEvent(NSEvent)

This action method dispatches mouse and keyboard events the global application object sends to the window.

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

