

- Core Data
- NSPersistentCloudKitContainer
-  eventNotificationUserInfoKey 

Type Property

# eventNotificationUserInfoKey

The user info dictionary key for the persistent CloudKit container event.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class let eventNotificationUserInfoKey: String
```

## See Also

### Monitoring Container Events

class Event

An object that represents activity in a persistent CloudKit container.

enum EventType

The type of event in a persistent CloudKit container, either setup, import, or export.

class NSPersistentCloudKitContainerEventRequest

A request to fetch setup, import, or export events in a persistent CloudKit container.

class NSPersistentCloudKitContainerEventResult

The result of a request to fetch persistent CloudKit container events.

class let eventChangedNotification: NSNotification.Name

A notification that contains details about an event in a persistent CloudKit container.

