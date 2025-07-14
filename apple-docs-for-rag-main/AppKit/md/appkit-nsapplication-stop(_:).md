

- AppKit
- NSApplication
-  stop(\_:) 

Instance Method

# stop(\_:)

Stops the main event loop.

macOS

``` source
@MainActor
func stop(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This method notifies the app that you want to exit the current run loop as soon as it finishes processing the current NSEvent object. This method doesn’t forcibly exit the current run loop. Instead it sets a flag that the app checks only after it finishes dispatching an actual event object. For example, you could call this method from an action method responding to a button click or from one of the many methods defined by the NSResponder class. However, calling this method from a timer or run-loop observer routine wouldn’t stop the run loop because they don’t result in the posting of an NSEvent object.

If you call this method from an event handler running in your main run loop, the app object exits out of the run() method, thereby returning control to the `main()` function. If you call this method from within a modal event loop, it will exit the modal loop instead of the main event loop.

## See Also

### Related Documentation

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

func terminate(Any?)

Terminates the receiver.

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

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

func sendEvent(NSEvent)

Dispatches an event to other objects.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

