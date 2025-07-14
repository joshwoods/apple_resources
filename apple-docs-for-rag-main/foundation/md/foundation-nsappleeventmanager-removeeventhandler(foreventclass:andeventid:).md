

- Foundation
- NSAppleEventManager
-  removeEventHandler(forEventClass:andEventID:) 

Instance Method

# removeEventHandler(forEventClass:andEventID:)

If an Apple event handler has been registered for the event specified by `eventClass` and `eventID`, removes it.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeEventHandler(
    forEventClass eventClass: AEEventClass,
    andEventID eventID: AEEventID
)
```

## Discussion

Otherwise does nothing.

## See Also

### Working with event handlers

func setEventHandler(Any, andSelector: Selector, forEventClass: AEEventClass, andEventID: AEEventID)

Registers the Apple event handler specified by `handler` for the event specified by `eventClass` and `eventID`.

