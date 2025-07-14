

- EventKit
-  EKObject 

Class

# EKObject

An abstract superclass for all EventKit classes that have persistent instances.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 6.0+

``` source
class EKObject
```

## Overview

`EKObject` provides fine control when saving and restoring property settings. For example, you can find out if a persistent object was modified locally and whether it needs to be saved. If the object has changed in the event store since it was fetched, you can refresh the local copy by keeping local changes or by removing local changes. You can also roll back the object to the state when it was first fetched.

## Topics

### Saving and Restoring State

var hasChanges: Bool

Returns whether this object or any of the objects it contains has uncommitted changes.

var isNew: Bool

A Boolean value that indicates whether this object has ever been saved.

func refresh() -> Bool

Merges changes to this object with the latest saved values.

func reset()

Returns this object to its saved state.

func rollback()

Rolls back the property values of this object to its original state when it was first fetched.

## Relationships

### Inherits From

- NSObject

### Inherited By

- EKAlarm
- EKCalendar
- EKCalendarItem
- EKParticipant
- EKRecurrenceRule
- EKSource
- EKStructuredLocation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Common objects

class EKCalendarItem

An abstract superclass for calendar events and reminders.

class EKSource

An abstract superclass that represents the account a calendar belongs to.

