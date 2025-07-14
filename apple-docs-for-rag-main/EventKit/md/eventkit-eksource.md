

- EventKit
-  EKSource 

Class

# EKSource

An abstract superclass that represents the account a calendar belongs to.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKSource
```

## Overview

You do not create instances of this class; instead, you retrieve `EKSource` objects from an EKEventStore object. Use the sources property to get all the `EKSource` objects for an event store, and use the methods in this class to access properties of the source object.

## Topics

### Accessing Source Properties

enum EKSourceType

The type of source object.

var sourceIdentifier: String

A unique identifier for the source object.

var sourceType: EKSourceType

The type of this source object.

var title: String

The name of this source object.

### Accessing Calendars

func calendars(for: EKEntityType) -> Set&lt;EKCalendar>

Returns the calendars that belong to this source object that support a particular entity type.

var calendars: Set&lt;EKCalendar>

The calendars that belong to this source object.

Deprecated

### Entity Type

enum EKEntityType

The type of entities allowed for a source.

### Instance Properties

var isDelegate: Bool

## Relationships

### Inherits From

- EKObject

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

class EKObject

An abstract superclass for all EventKit classes that have persistent instances.

