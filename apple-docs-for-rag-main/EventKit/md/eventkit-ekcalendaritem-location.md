

- EventKit
- EKCalendarItem
-  location 

Instance Property

# location

The location associated with the calendar item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var location: String? { get set }
```

## Discussion

This property is `nil` if the calendar item has no location.

## See Also

### Accessing Calendar Item Properties

var calendar: EKCalendar!

The calendar for the calendar item.

var title: String!

The title for the calendar item.

var creationDate: Date?

The date that this calendar item was created.

var lastModifiedDate: Date?

The date that the calendar item was last modified.

var timeZone: TimeZone?

The time zone for the calendar item.

var url: URL?

The URL for the calendar item.

