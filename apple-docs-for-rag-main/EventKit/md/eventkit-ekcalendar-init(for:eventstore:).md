

- EventKit
- EKCalendar
-  init(for:eventStore:) 

Initializer

# init(for:eventStore:)

Creates a new calendar that can contain the given entity type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
init(
    for entityType: EKEntityType,
    eventStore: EKEventStore
)
```

## Parameters 

`entityType`  

The entity type that this calendar may support.

`eventStore`  

The event store in which to create this calendar.

## Return Value

The created calendar.

## Discussion

You can only create calendars that accept either reminders or events. Some servers might allow mixing the two, although it is not common.

## See Also

### Creating Calendars

init(eventStore: EKEventStore)

Creates and returns a calendar belonging to a specified event store.

Deprecated

