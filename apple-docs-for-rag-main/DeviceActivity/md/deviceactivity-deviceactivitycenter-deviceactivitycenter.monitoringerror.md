

- DeviceActivity
- DeviceActivityCenter
-  DeviceActivityCenter.MonitoringError 

Enumeration

# DeviceActivityCenter.MonitoringError

Errors that may occur when starting to monitor an activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum MonitoringError
```

## Topics

### Checking for Errors

case excessiveActivities

The calling process is monitoring too many activities.

case intervalTooLong

The activity’s schedule has an interval that is too long.

case intervalTooShort

The activity’s schedule has an interval that is too short.

case invalidDateComponents

The schedule’s date range is invalid.

case unauthorized

The calling process isn’t authorized to monitor device activity.

### Getting the Localized Message

var errorDescription: String?

A localized message that describes what error occurred.

var failureReason: String?

A localized message that describes the reason for the failure.

var helpAnchor: String?

A localized message that provides a help text if the user requests help.

var localizedDescription: String

A string that contains the localized description of the error.

var recoverySuggestion: String?

A localized message that describes how to recover from the failure.

### Comparing Errors

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

### Operators

static func == (DeviceActivityCenter.MonitoringError, DeviceActivityCenter.MonitoringError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

