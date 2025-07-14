

- EventKit
-  EKParticipant 

Class

# EKParticipant

A class that represents person, group, or room invited to a calendar event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKParticipant
```

## Overview

Do not create `EKParticipant` objects directly. Instead, use the property attendees on EKCalendarItem to return an array of `EKParticipant` objects.

EventKit cannot add participants to an event nor change participant information. Use the properties in this class to get information about a participant.

A participant can be a person, group, room, or other resource.

## Topics

### Defining Participants

enum EKParticipantRole

The participant’s role for an event.

enum EKParticipantType

The type of participant.

enum EKParticipantStatus

The participant’s attendance status for an event.

enum EKParticipantScheduleStatus

The participant’s scheduled status.

### Accessing Participant Properties

var isCurrentUser: Bool

A Boolean value indicating whether this participant represents the owner of this account.

var name: String?

The participant’s name.

var participantRole: EKParticipantRole

The participant’s role in the event.

var participantStatus: EKParticipantStatus

The participant’s attendance status.

var participantType: EKParticipantType

The participant’s type.

var url: URL

The URL representing this participant.

var contactPredicate: NSPredicate

A predicate to use with the Contacts framework to retrieve the corresponding contact instance.

### Finding Participant Address Book Records

func abRecord(with: ABAddressBook) -> ABRecord?

Returns the address book record that represents the participant.

func abPerson(in: ABAddressBook) -> ABPerson?

Returns the address book record that represents the participant.

Deprecated

typealias ABAddressBook

A reference to an ABAddressBook object.

Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

## Relationships

### Inherits From

- EKObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Calendars

class EKCalendar

A class that represents a calendar in EventKit.

