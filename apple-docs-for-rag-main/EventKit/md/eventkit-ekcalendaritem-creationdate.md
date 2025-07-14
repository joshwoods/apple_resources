

- EventKit
- EKCalendarItem
-  creationDate 

Instance Property

# creationDate

The date that this calendar item was created.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var creationDate: Date? { get }
```

## Discussion

If `nil`, this property was not set or was synced in this state.

## See Also

### Accessing Calendar Item Properties

var calendar: EKCalendar!

The calendar for the calendar item.

var title: String!

The title for the calendar item.

var location: String?

The location associated with the calendar item.

var lastModifiedDate: Date?

The date that the calendar item was last modified.

var timeZone: TimeZone?

The time zone for the calendar item.

var url: URL?

The URL for the calendar item.

