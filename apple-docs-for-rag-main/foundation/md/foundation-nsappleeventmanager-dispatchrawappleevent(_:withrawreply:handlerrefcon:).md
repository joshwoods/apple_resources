

- Foundation
- NSAppleEventManager
-  dispatchRawAppleEvent(\_:withRawReply:handlerRefCon:) 

Instance Method

# dispatchRawAppleEvent(\_:withRawReply:handlerRefCon:)

Causes the Apple event specified by `theAppleEvent` to be dispatched to the appropriate Apple event handler, if one has been registered by calling setEventHandler(_:andSelector:forEventClass:andEventID:).

Mac Catalyst 13.0+macOS 10.0+

``` source
func dispatchRawAppleEvent(
    _ theAppleEvent: UnsafePointer,
    withRawReply theReply: UnsafeMutablePointer,
    handlerRefCon: SRefCon
) -> OSErr
```

## Discussion

The `theReply` parameter always specifies a reply Apple event, never `nil`. However, the handler should not fill out the reply if the descriptor type for the reply event is `typeNull`, indicating the sender does not want a reply.

The `handlerRefcon` parameter provides 4 bytes of data to the handler; a common use for this parameter is to pass a pointer to additional data.

This method is primarily intended for Cocoa’s internal use. Note that *dispatching* an event means routing an event to an appropriate handler in the current application. You cannot use this method to *send* an event to other applications.

