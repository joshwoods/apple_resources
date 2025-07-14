

- AppKit
- NSApplication
-  run() 

Instance Method

# run()

Starts the main event loop.

macOS

``` source
@MainActor
func run()
```

## Discussion

The loop continues until a stop(_:) or terminate(_:) message is received. Upon each iteration through the loop, the next available event from the window server is stored and then dispatched by sending it to `NSApp` using sendEvent(_:).

After creating the `NSApplication` object, the `main` function should load your app’s main nib file and then start the event loop by sending the `NSApplication` object a run() message. If you create an Cocoa app project in Xcode, this `main` function is implemented for you.

## See Also

### Related Documentation

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

func applicationDidFinishLaunching(Notification)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

### Managing the Event Loop

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Removes all events matching the given mask and generated before the specified event.

var currentEvent: NSEvent?

The last event object that the app retrieved from the event queue.

var isRunning: Bool

A Boolean value indicating whether the main event loop is running.

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

func stop(Any?)

Stops the main event loop.

func sendEvent(NSEvent)

Dispatches an event to other objects.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

