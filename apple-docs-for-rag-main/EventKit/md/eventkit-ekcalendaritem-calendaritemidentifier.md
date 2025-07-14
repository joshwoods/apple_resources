

- EventKit
- EKCalendarItem
-  calendarItemIdentifier 

Instance Property

# calendarItemIdentifier

The calendar item’s unique identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var calendarItemIdentifier: String { get }
```

## Discussion

This property is set when the calendar item is created and can be used as a local identifier. Use calendarItem(withIdentifier:) to look up the item by this value.

A full sync with the calendar will lose this identifier. You should have a plan for dealing with a calendar whose identifier is no longer fetch-able by caching its other properties.

## See Also

### Related Documentation

var calendarIdentifier: String

A unique identifier for the calendar.

Calendar and Reminders Programming Guide

### Accessing Calendar Items

var calendarItemExternalIdentifier: String!

The calendar item’s external identifier as provided by the calendar server.

var uuid: String

The calendar item’s unique identifier.

Deprecated

