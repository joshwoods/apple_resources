

- EventKit
- EKCalendarItem
-  attendees 

Instance Property

# attendees

The attendees associated with the calendar item, as an array of EKParticipant objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var attendees: [EKParticipant]? { get }
```

## Discussion

This property is read-only; it is not possible to add attendees with Event Kit. This property is `nil` if the calendar item has no attendees.

## See Also

### Displaying Attendees

var hasAttendees: Bool

A Boolean value that indicates whether the calendar item has attendees.

