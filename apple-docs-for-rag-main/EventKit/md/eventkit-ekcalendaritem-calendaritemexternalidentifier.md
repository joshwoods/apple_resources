

- EventKit
- EKCalendarItem
-  calendarItemExternalIdentifier 

Instance Property

# calendarItemExternalIdentifier

The calendar item’s external identifier as provided by the calendar server.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var calendarItemExternalIdentifier: String! { get }
```

## Discussion

This identifier allows you to access the same event or reminder across multiple devices.

There are some cases where duplicate copies of a calendar item can exist in the same database:

- A calendar item was imported from an ICS file into multiple calendars

- An event was created in a calendar shared with the user and the user was also invited to the event

- The user is a delegate of a calendar that also has this event

- A subscribed calendar was added to multiple accounts

In such cases, you should choose between calendar items based on other factors, such as the calendar or source.

Recurring event identifiers are the same for all occurrences. If you wish to differentiate between occurrences, you may want to use the start date.

For Exchange servers, the identifier is different between iOS and macOS and different between devices for reminders.

## See Also

### Accessing Calendar Items

var calendarItemIdentifier: String

The calendar item’s unique identifier.

var uuid: String

The calendar item’s unique identifier.

Deprecated

