

- AppKit
- NSApplication
-  sendEvent(\_:) 

Instance Method

# sendEvent(\_:)

Dispatches an event to other objects.

macOS

``` source
@MainActor
func sendEvent(_ event: NSEvent)
```

## Parameters 

`event`  

The event object to dispatch.

## Discussion

You rarely invoke sendEvent(_:) directly, although you might want to override this method to perform some action on every event. sendEvent(_:) messages are sent from the main event loop (the run() method). sendEvent(_:) is the method that dispatches events to the appropriate responders—`NSApp` handles app events, the NSWindow object indicated in the event record handles window-related events, and mouse and key events are forwarded to the appropriate NSWindow object for further dispatching.

## See Also

### Managing the Event Loop

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Removes all events matching the given mask and generated before the specified event.

var currentEvent: NSEvent?

The last event object that the app retrieved from the event queue.

var isRunning: Bool

A Boolean value indicating whether the main event loop is running.

func run()

Starts the main event loop.

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

func stop(Any?)

Stops the main event loop.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

