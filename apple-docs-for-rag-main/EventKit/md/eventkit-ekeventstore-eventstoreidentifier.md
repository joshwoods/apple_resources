

- EventKit
- EKEventStore
-  eventStoreIdentifier 

Instance Property

# eventStoreIdentifier

The unique identifier for the event store.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var eventStoreIdentifier: String { get }
```

## Discussion

If the store is damaged, it’s recreated and given a new identifier. If this value is different from a fetched value, you should take the appropriate action.

## See Also

### Creating event stores

init()

Creates a new event store.

init(sources: [EKSource])

Creates an event store that contains data for the specified sources.

