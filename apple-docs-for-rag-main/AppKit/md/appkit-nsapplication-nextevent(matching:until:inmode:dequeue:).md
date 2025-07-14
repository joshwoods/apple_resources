

- AppKit
- NSApplication
-  nextEvent(matching:until:inMode:dequeue:) 

Instance Method

# nextEvent(matching:until:inMode:dequeue:)

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

macOS

``` source
@MainActor
func nextEvent(
    matching mask: NSEvent.EventTypeMask,
    until expiration: Date?,
    inMode mode: RunLoop.Mode,
    dequeue deqFlag: Bool
) -> NSEvent?
```

## Parameters 

`mask`  

Contains one or more flags indicating the types of events to return. The constants section of the NSEvent class defines the constants you can add together to create this mask. The discardEvents(matching:before:) method also lists several of these constants.

`expiration`  

The expiration date for the current event request. Specifying nil for this parameter is equivalent to returning a date object using the distantPast method.

`mode`  

The run loop mode in which to run while looking for events. The mode you specify also determines which timers and run-loop observers may fire while the app waits for the event.

`deqFlag`  

Specify true if you want the event removed from the queue.

## Return Value

The event object whose type matches one of the event types specified by the `mask` parameter.

## Discussion

You can use this method to short circuit normal event dispatching and get your own events. For example, you may want to do this in response to a mouse-down event in order to track the mouse while its button is down. (In such an example, you’d pass the appropriate event types for mouse-dragged and mouse-up events to the `mask` parameter and specify the `NSEventTrackingRunLoopMode` run loop mode). Events that don’t match one of the specified event types are left in the queue.

You can specify one of the run loop modes defined by AppKit or a custom run loop mode used specifically by your app. AppKit defines the following run-loop modes:

- `NSDefaultRunLoopMode`

- `NSEventTrackingRunLoopMode`

- `NSModalPanelRunLoopMode`

- `NSConnectionReplyMode`

## See Also

### Related Documentation

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

### Managing the Event Loop

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

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

