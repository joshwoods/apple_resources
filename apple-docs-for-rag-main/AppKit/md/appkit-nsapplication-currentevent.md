

- AppKit
- NSApplication
-  currentEvent 

Instance Property

# currentEvent

The last event object that the app retrieved from the event queue.

macOS

``` source
@MainActor
var currentEvent: NSEvent? { get }
```

## Discussion

The shared app object receives events and forwards them to the affected NSWindow objects, which then distribute them to the objects in its view hierarchy. Use this property to get the event that was last handled by the app.

## See Also

### Managing the Event Loop

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Removes all events matching the given mask and generated before the specified event.

var isRunning: Bool

A Boolean value indicating whether the main event loop is running.

func run()

Starts the main event loop.

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

func stop(Any?)

Stops the main event loop.

func sendEvent(NSEvent)

Dispatches an event to other objects.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

