

- EventKit
- EKEventStore
-  delegateSources 

Instance Property

# delegateSources

The event sources delegated to the person using your app.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 5.0+

``` source
var delegateSources: [EKSource] { get }
```

## Discussion

By default, delegate event sources aren’t included in an event store’s sources. To access events and reminders in a delegate source:

1.  Use init() to initialize an EKEventStore.

2.  Use requestAccess(to:completion:) to request access to the desired entity types.

3.  Get the delegate sources from the event store using delegateSources.

4.  After the request is granted, initialize another EKEventStore using init(sources:), passing the delegate stores.

## See Also

### Accessing account sources

var sources: [EKSource]

An unordered array of objects that represent accounts that contain calendars.

func source(withIdentifier: String) -> EKSource?

Locates an event source with the specified identifier.

