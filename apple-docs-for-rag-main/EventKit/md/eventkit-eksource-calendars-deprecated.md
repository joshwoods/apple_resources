

- EventKit
- EKSource
-  calendars Deprecated

Instance Property

# calendars

The calendars that belong to this source object.

watchOS 2.0–2.0Deprecated

``` source
var calendars: Set { get }
```

## Discussion

Note

This property is not available in macOS.

## See Also

### Accessing Calendars

func calendars(for: EKEntityType) -> Set&lt;EKCalendar>

Returns the calendars that belong to this source object that support a particular entity type.

