

- Core Data
- NSPersistentCloudKitContainer
- NSPersistentCloudKitContainer.Event
-  error 

Instance Property

# error

An error that indicates why an operation fails.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var error: (any Error)? { get }
```

## See Also

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

