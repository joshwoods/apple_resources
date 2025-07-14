

- AppKit
- NSApplication
-  postEvent(\_:atStart:) 

Instance Method

# postEvent(\_:atStart:)

Adds a given event to the receiver’s event queue.

macOS

``` source
@MainActor
func postEvent(
    _ event: NSEvent,
    atStart: Bool
)
```

## Parameters 

`event`  

The event object to post to the queue.

`atStart`  

Specify true to add the event to the front of the queue; otherwise, specify false to add the event to the back of the queue.

## Discussion

This method can also be called in subthreads. Events posted in subthreads bubble up in the main thread event queue.

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

func sendEvent(NSEvent)

Dispatches an event to other objects.

