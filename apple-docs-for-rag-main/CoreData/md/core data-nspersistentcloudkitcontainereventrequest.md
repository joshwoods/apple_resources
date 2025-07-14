

- Core Data
-  NSPersistentCloudKitContainerEventRequest 

Class

# NSPersistentCloudKitContainerEventRequest

A request to fetch setup, import, or export events in a persistent CloudKit container.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class NSPersistentCloudKitContainerEventRequest
```

## Topics

### Fetching Events

class func fetchEvents(after: Date) -> Self

Creates a fetch request for events after a specified date from a persistent CloudKit container.

class func fetchEvents(after: NSPersistentCloudKitContainer.Event?) -> Self

Creates a fetch request for events that occur after a specified event from a persistent CloudKit container.

class func fetchEvents(matchingFetch: NSFetchRequest&lt;any NSFetchRequestResult>) -> Self

Creates a fetch request for events that match a specified fetch request from a persistent CloudKit container.

class func fetchForEvents() -> NSFetchRequest&lt;any NSFetchRequestResult>

Creates a fetch request for all events in a persistent CloudKit container.

var resultType: NSPersistentCloudKitContainerEventResult.ResultType

The type of result that the request returns.

## Relationships

### Inherits From

- NSPersistentStoreRequest

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

class Event

An object that represents activity in a persistent CloudKit container.

enum EventType

The type of event in a persistent CloudKit container, either setup, import, or export.

class NSPersistentCloudKitContainerEventResult

The result of a request to fetch persistent CloudKit container events.

class let eventChangedNotification: NSNotification.Name

A notification that contains details about an event in a persistent CloudKit container.

class let eventNotificationUserInfoKey: String

The user info dictionary key for the persistent CloudKit container event.

