

- AppKit
- NSWindow
-  tryToPerform(\_:with:) 

Instance Method

# tryToPerform(\_:with:)

Dispatches action messages with a given argument.

macOS

``` source
@MainActor
func tryToPerform(
    _ action: Selector,
    with object: Any?
) -> Bool
```

## Parameters 

`action`  

The selector to attempt to execute.

`object`  

The message’s argument.

## Return Value

true when the window or its delegate perform `action` with `object`; otherwise, false.

## Discussion

The window tries to perform the method `action` using its inherited `NSResponder` method tryToPerform(_:with:). If the window doesn’t perform `action`, the delegate is given the opportunity to perform it using its inherited `NSObject` method perform(_:with:).

## See Also

### Handling Events

var currentEvent: NSEvent?

The event currently being processed by the application.

func nextEvent(matching: NSEvent.EventTypeMask) -> NSEvent?

Returns the next event matching a given mask.

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Forwards the message to the global application object.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Forwards the message to the global application object.

func postEvent(NSEvent, atStart: Bool)

Forwards the message to the global application object.

func sendEvent(NSEvent)

This action method dispatches mouse and keyboard events the global application object sends to the window.

