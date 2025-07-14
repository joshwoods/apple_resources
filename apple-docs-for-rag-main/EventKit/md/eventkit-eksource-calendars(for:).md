

- EventKit
- EKSource
-  calendars(for:) 

Instance Method

# calendars(for:)

Returns the calendars that belong to this source object that support a particular entity type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func calendars(for entityType: EKEntityType) -> Set
```

## Parameters 

`entityType`  

The entity type of either an event or a reminder.

## Return Value

The calendars belonging to this source that support the entity type.

## See Also

### Related Documentation

struct EKEntityMask

A bitmask of `EKEntityType` for specifying multiple entities at once.

### Accessing Calendars

var calendars: Set&lt;EKCalendar>

The calendars that belong to this source object.

Deprecated

