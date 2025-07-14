

- EventKit
- EKEvent
-  structuredLocation 

Instance Property

# structuredLocation

The event’s location with a potential geocoordinate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var structuredLocation: EKStructuredLocation? { get set }
```

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

var occurrenceDate: Date!

The original occurrence date of an event if it is part of a recurring series.

var isDetached: Bool

A Boolean value that indicates whether an event is a detached instance of a repeating event.

var organizer: EKParticipant?

The organizer associated with the event.

var status: EKEventStatus

The status of the event.

var birthdayContactIdentifier: String?

The contact identifier of the person for this birthday event.

var birthdayPersonID: Int

The Address Book framework record identifier of the person for this birthday event.

Deprecated

var birthdayPersonUniqueID: String?

The Address Book framework record identifier of the person for this birthday event.

Deprecated

