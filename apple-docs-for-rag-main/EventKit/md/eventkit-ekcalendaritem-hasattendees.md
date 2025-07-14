

- EventKit
- EKCalendarItem
-  hasAttendees 

Instance Property

# hasAttendees

A Boolean value that indicates whether the calendar item has attendees.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var hasAttendees: Bool { get }
```

## Discussion

If true, the calendar item has attendees; otherwise it does not.

## See Also

### Displaying Attendees

var attendees: [EKParticipant]?

The attendees associated with the calendar item, as an array of EKParticipant objects.

