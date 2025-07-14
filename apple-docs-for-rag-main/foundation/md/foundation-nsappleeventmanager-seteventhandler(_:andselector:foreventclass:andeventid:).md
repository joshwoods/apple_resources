

- Foundation
- NSAppleEventManager
-  setEventHandler(\_:andSelector:forEventClass:andEventID:) 

Instance Method

# setEventHandler(\_:andSelector:forEventClass:andEventID:)

Registers the Apple event handler specified by `handler` for the event specified by `eventClass` and `eventID`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setEventHandler(
    _ handler: Any,
    andSelector handleEventSelector: Selector,
    forEventClass eventClass: AEEventClass,
    andEventID eventID: AEEventID
)
```

## Discussion

If an event handler is already registered for the specified event class and event ID, removes it. The signature for `handler` should match the following:

```
- (void)handleAppleEvent:(NSAppleEventDescriptor *)event withReplyEvent: (NSAppleEventDescriptor *)replyEvent;
```

## See Also

### Working with event handlers

func removeEventHandler(forEventClass: AEEventClass, andEventID: AEEventID)

If an Apple event handler has been registered for the event specified by `eventClass` and `eventID`, removes it.

