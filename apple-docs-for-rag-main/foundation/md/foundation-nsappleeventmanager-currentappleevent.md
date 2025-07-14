

- Foundation
- NSAppleEventManager
-  currentAppleEvent 

Instance Property

# currentAppleEvent

Returns the descriptor for `currentAppleEvent` if an Apple event is being handled on the current thread.

Mac Catalyst 13.0+macOS 10.0+

``` source
var currentAppleEvent: NSAppleEventDescriptor? { get }
```

## Discussion

An Apple event is being handled on the current thread if a handler that was registered with setEventHandler(_:andSelector:forEventClass:andEventID:) is being messaged at this instant or setCurrentAppleEventAndReplyEventWithSuspensionID(_:) has just been invoked. Returns `nil` otherwise. The effects of mutating or retaining the returned descriptor are undefined, although it may be copied.

## See Also

### Suspending and resuming Apple events

func appleEvent(forSuspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the descriptor for the event whose handling was suspended.

var currentReplyAppleEvent: NSAppleEventDescriptor?

Returns the corresponding reply event descriptor if an Apple event is being handled on the current thread.

func replyAppleEvent(forSuspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the corresponding reply event descriptor.

func resume(withSuspensionID: NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), signal that handling of the suspended event may now continue.

func setCurrentAppleEventAndReplyEventWithSuspensionID(NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), sets the values that will be returned by subsequent invocations of currentAppleEvent and currentReplyAppleEvent to be the event whose handling was suspended and its corresponding reply event, respectively.

func suspendCurrentAppleEvent() -> NSAppleEventManager.SuspensionID?

Suspends the handling of the current event and returns an ID that must be used to resume the handling of the event if an Apple event is being handled on the current thread.

typealias SuspensionID

Identifies an Apple event whose handling has been suspended. Can be used to resume handling of the Apple event.

