

- AppKit
- NSWindow
-  nextEvent(matching:) 

Instance Method

# nextEvent(matching:)

Returns the next event matching a given mask.

macOS

``` source
@MainActor
func nextEvent(matching mask: NSEvent.EventTypeMask) -> NSEvent?
```

## Parameters 

`mask`  

The mask that the event to return must match. Events with non-matching masks are left in the queue. See discardEvents(matching:before:) in NSApplication for the list of mask values.

## Return Value

The next event whose mask matches `mask`; `nil` when no matching event was found.

## Discussion

This method calls the nextEvent(matching:until:inMode:dequeue:) method, where the matching mask parameter is the specified `mask`, the `until` (Swift) or `untilDate` (Objective-C) parameter is distantFuture, the `inMode` parameter is NSEventTrackingRunLoopMode, and the `dequeue` parameter is true.

## See Also

### Related Documentation

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

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

