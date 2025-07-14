

- EventKit
- EKEvent
-  birthdayPersonUniqueID Deprecated

Instance Property

# birthdayPersonUniqueID

The Address Book framework record identifier of the person for this birthday event.

macOS 10.8–10.11Deprecated

``` source
var birthdayPersonUniqueID: String? { get }
```

Deprecated

Use birthdayContactIdentifier instead

## Discussion

This property is only set if this is a birthday event; otherwise the property is `nil`.

### Special Considerations

Note

This property is equivalent to the birthdayPersonID property on iOS.

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

var structuredLocation: EKStructuredLocation?

The event’s location with a potential geocoordinate.

var birthdayPersonID: Int

The Address Book framework record identifier of the person for this birthday event.

Deprecated

