

- EventKit
-  EKEvent 

Class

# EKEvent

A class that represents an event in a calendar.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKEvent
```

## Mentioned in 

Creating events and reminders

Retrieving events and reminders

## Overview

Use the init(eventStore:) method to create a new event. Use the properties in the class to get and modify certain information about an event. Other properties, such as the event’s title and calendar, are inherited from the parent class EKCalendarItem.

## Topics

### Creating Events

init(eventStore: EKEventStore)

Creates and returns a new event belonging to a specified event store.

### Scheduling Events

enum EKEventStatus

The event’s status.

enum EKEventAvailability

The event’s availability setting for scheduling purposes.

### Comparing Events

func compareStartDate(with: EKEvent) -> ComparisonResult

Compares the start date of the receiving event with the start date of another event.

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

var birthdayPersonUniqueID: String?

The Address Book framework record identifier of the person for this birthday event.

Deprecated

### Refreshing Event Data

func refresh() -> Bool

Updates the event’s data with the current information in the Calendar database.

## Relationships

### Inherits From

- EKCalendarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Events and reminders

Creating events and reminders

Create and modify events and reminders in a person’s database.

Retrieving events and reminders

Fetch events and reminders from the Calendar database.

Updating with notifications

Register for notifications about changes and keep your app up to date.

Managing Location-Based Reminders

Add, fetch, complete, remove, and sort location-based reminders in your app.

class EKReminder

A class that represents a reminder in a calendar.

