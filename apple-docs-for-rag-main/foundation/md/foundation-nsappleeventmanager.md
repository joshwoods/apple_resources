

- Foundation
-  NSAppleEventManager 

Class

# NSAppleEventManager

A mechanism for registering handler routines for specific types of Apple events and dispatching events to those handlers.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSAppleEventManager
```

## Overview

Cocoa provides built-in scriptability support that uses scriptability information supplied by an application to automatically convert Apple events into script command objects that perform the desired operation. However, some applications may want to perform more basic Apple event handling, in which an application registers handlers for the Apple events it can process, then calls on the Apple Event Manager to dispatch received Apple events to the appropriate handler. `NSAppleEventManager` supports these mechanisms by providing methods to register and remove handlers and to dispatch Apple events to the appropriate handler, if one exists. For related information, see How Cocoa Applications Handle Apple Events

Each application has at most one instance of `NSAppleEventManager`. To obtain a reference to it, you call the class method shared(), which creates the instance if it doesn’t already exist.

For information about the Apple Event Manager, see Apple Event Manager and Apple Events Programming Guide.

## Topics

### Getting an event manager

class func shared() -> NSAppleEventManager

Returns the single instance of `NSAppleEventManager`, creating it first if it doesn’t exist.

### Working with event handlers

func removeEventHandler(forEventClass: AEEventClass, andEventID: AEEventID)

If an Apple event handler has been registered for the event specified by `eventClass` and `eventID`, removes it.

func setEventHandler(Any, andSelector: Selector, forEventClass: AEEventClass, andEventID: AEEventID)

Registers the Apple event handler specified by `handler` for the event specified by `eventClass` and `eventID`.

### Working with events

func dispatchRawAppleEvent(UnsafePointer&lt;AppleEvent>, withRawReply: UnsafeMutablePointer&lt;AppleEvent>, handlerRefCon: SRefCon) -> OSErr

Causes the Apple event specified by `theAppleEvent` to be dispatched to the appropriate Apple event handler, if one has been registered by calling setEventHandler(_:andSelector:forEventClass:andEventID:).

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

func suspendCurrentAppleEvent() -> NSAppleEventManager.SuspensionID?

Suspends the handling of the current event and returns an ID that must be used to resume the handling of the event if an Apple event is being handled on the current thread.

typealias SuspensionID

Identifies an Apple event whose handling has been suspended. Can be used to resume handling of the Apple event.

### Constants

NSAppleEvent Timeouts

The following constants should not be used and may eventually be removed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Apple Event Handling

class NSAppleEventDescriptor

A wrapper for the Apple event descriptor data type.

