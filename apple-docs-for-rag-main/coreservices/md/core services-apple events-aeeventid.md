

- Core Services
- Apple Events
-  AEEventID 

Type Alias

# AEEventID

Specifies the event ID of an Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEEventID = FourCharCode
```

## Discussion

Apple events are identified by their event class and event ID attributes. The event ID is the attribute that identifies a particular Apple event within its event class. In conjunction with the event class, the event ID uniquely identifies the Apple event and communicates what action the Apple event should perform.

For more information on Apple event IDs, see Event ID Constants.

