

- AppKit
- NSApplication
-  finishLaunching() 

Instance Method

# finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

macOS

``` source
@MainActor
func finishLaunching()
```

## Discussion

The run() method calls this method before it starts the event loop. When this method begins, it posts an willFinishLaunchingNotification to the default notification center. If you override finishLaunching(), the subclass method should invoke the superclass method.

## See Also

### Related Documentation

func applicationWillFinishLaunching(Notification)

Tells the delegate that the app’s initialization is about to complete.

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

func run()

Starts the main event loop.

func stop(Any?)

Stops the main event loop.

func sendEvent(NSEvent)

Dispatches an event to other objects.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

