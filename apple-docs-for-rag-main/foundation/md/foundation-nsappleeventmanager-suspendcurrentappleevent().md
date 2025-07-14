

- Foundation
- NSAppleEventManager
-  suspendCurrentAppleEvent() 

Instance Method

# suspendCurrentAppleEvent()

Suspends the handling of the current event and returns an ID that must be used to resume the handling of the event if an Apple event is being handled on the current thread.

Mac Catalyst 13.0+macOS 10.0+

``` source
func suspendCurrentAppleEvent() -> NSAppleEventManager.SuspensionID?
```

## Discussion

An Apple event is being handled on the current thread if currentAppleEvent does not return `nil`. Returns zero otherwise. The suspended event is no longer the current event after this method returns.

## See Also

### Suspending and resuming Apple events

func appleEvent(forSuspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the descriptor for the event whose handling was suspended.

var currentAppleEvent: NSAppleEventDescriptor?

Returns the descriptor for `currentAppleEvent` if an Apple event is being handled on the current thread.

var currentReplyAppleEvent: NSAppleEventDescriptor?

Returns the corresponding reply event descriptor if an Apple event is being handled on the current thread.

func replyAppleEvent(forSuspensionID: NSAppleEventManager.SuspensionID) -> NSAppleEventDescriptor

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), returns the corresponding reply event descriptor.

func resume(withSuspensionID: NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), signal that handling of the suspended event may now continue.

func setCurrentAppleEventAndReplyEventWithSuspensionID(NSAppleEventManager.SuspensionID)

Given a nonzero `suspensionID` returned by an invocation of suspendCurrentAppleEvent(), sets the values that will be returned by subsequent invocations of currentAppleEvent and currentReplyAppleEvent to be the event whose handling was suspended and its corresponding reply event, respectively.

typealias SuspensionID

Identifies an Apple event whose handling has been suspended. Can be used to resume handling of the Apple event.

