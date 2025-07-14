

- Core Services
- Apple Events
-  AEEventClass 

Type Alias

# AEEventClass

Specifies the event class of an Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEEventClass = FourCharCode
```

## Discussion

Apple events are identified by their event class and event ID attributes. The event class is the attribute that identifies a group of related Apple events. When you call the `AEProcessAppleEvent(_:)` function, the Apple Event Manager uses these attributes to identify a handler for a specific Apple event.

For more information on Apple event classes, see Event Class Constants.

