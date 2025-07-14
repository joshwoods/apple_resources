

- Core Data
- NSPersistentCloudKitContainer
-  NSPersistentCloudKitContainer.Event 

Class

# NSPersistentCloudKitContainer.Event

An object that represents activity in a persistent CloudKit container.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class Event
```

## Topics

### Inspecting Event Properties

var type: NSPersistentCloudKitContainer.EventType

The type of event, either setup, import, or export.

var identifier: UUID

A unique identifier for the event in a container.

var storeIdentifier: String

The associated store identifier in the container for the event.

var succeeded: Bool

A Boolean value that indicates whether the operation the event represents is successful.

var startDate: Date

The start date of the operation that the event represents.

var endDate: Date?

The end date of the operation that the event represents.

var error: (any Error)?

An error that indicates why an operation fails.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Monitoring Container Events

enum EventType

The type of event in a persistent CloudKit container, either setup, import, or export.

class NSPersistentCloudKitContainerEventRequest

A request to fetch setup, import, or export events in a persistent CloudKit container.

class NSPersistentCloudKitContainerEventResult

The result of a request to fetch persistent CloudKit container events.

class let eventChangedNotification: NSNotification.Name

A notification that contains details about an event in a persistent CloudKit container.

class let eventNotificationUserInfoKey: String

The user info dictionary key for the persistent CloudKit container event.

