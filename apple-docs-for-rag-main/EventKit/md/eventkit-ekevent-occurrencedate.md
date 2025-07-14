

- EventKit
- EKEvent
-  occurrenceDate 

Instance Property

# occurrenceDate

The original occurrence date of an event if it is part of a recurring series.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var occurrenceDate: Date! { get }
```

## Discussion

This value remains the same even when the event has been detached and its start date has changed. Floating events (such as all-day events) are returned in the default time zone.

## See Also

### Accessing Event Properties

var eventIdentifier: String!

A unique identifier for the event.

var availability: EKEventAvailability

The availability setting for the event.

var startDate: Date!

The start date of the event.

var endDate: Date!

The end date for the event.

var isAllDay: Bool

A Boolean value that indicates whether the event is an all-day event.

var isDetached: Bool

A Boolean value that indicates whether an event is a detached instance of a repeating event.

var organizer: EKParticipant?

The organizer associated with the event.

var status: EKEventStatus

The status of the event.

var birthdayContactIdentifier: String?

The contact identifier of the person for this birthday event.

var structuredLocation: EKStructuredLocation?

The event’s location with a potential geocoordinate.

var birthdayPersonID: Int

The Address Book framework record identifier of the person for this birthday event.

Deprecated

var birthdayPersonUniqueID: String?

The Address Book framework record identifier of the person for this birthday event.

Deprecated

