

- Foundation
- NSAppleEventManager
-  replyAppleEvent(forSuspensionID:) 

Instance Method

# replyAppleEvent(forSuspensionID:)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the corresponding reply event descriptor.

Mac Catalyst 13.0+macOS 10.0+

``` source
func replyAppleEvent(forSuspensionID suspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor
```

## Discussion

This descriptor, including any mutations, will be returned to the sender of the suspended event when handling of the event is resumed, if the sender has requested a reply. The effects of retaining the descriptor are undefined; it may be copied, but mutations of the copy are returned to the sender of the suspended event. replyAppleEvent(forSuspensionID:) may be invoked in any thread, not just the one in which the corresponding invocation of suspendCurrentAppleEvent() occurred.

## See Also

### Suspending and resuming Apple events

func appleEvent(forSuspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the descriptor for the event whose handling was suspended.

var currentAppleEvent: NSAppleEventDescriptor?

Returns the descriptor for `currentAppleEvent` if an Apple event is being handled on the current thread.

var currentReplyAppleEvent: NSAppleEventDescriptor?

Returns the corresponding reply event descriptor if an Apple event is being handled on the current thread.

func resume(withSuspensionID: NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), signal that handling of the suspended event may now continue.

func setCurrentAppleEventAndReplyEventWithSuspensionID(NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), sets the values that will be returned by subsequent invocations of currentAppleEvent and currentReplyAppleEvent to be the event whose handling was suspended and its corresponding reply event, respectively.

func suspendCurrentAppleEvent() -> NSAppleEventManager.SuspensionID?

Suspends the handling of the current event and returns an ID that must be used to resume the handling of the event if an Apple event is being handled on the current thread.

typealias SuspensionID

Identifies an Apple event whose handling has been suspended. Can be used to resume handling of the Apple event.

