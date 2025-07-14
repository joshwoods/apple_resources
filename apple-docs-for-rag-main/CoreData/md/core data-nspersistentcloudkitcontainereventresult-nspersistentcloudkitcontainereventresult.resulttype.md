

- Core Data
- NSPersistentCloudKitContainerEventResult
-  NSPersistentCloudKitContainerEventResult.ResultType 

Enumeration

# NSPersistentCloudKitContainerEventResult.ResultType

The types of results from a persistent CloudKit container event fetch request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum ResultType
```

## Topics

### Result Types

case events

The persistent CloudKit container events that match the event request.

case countEvents

The number of CloudKit container events that match the event request.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Event Results

var result: Any?

The result of the persistent CloudKit container event request, which the result type determines.

var resultType: NSPersistentCloudKitContainerEventResult.ResultType

The type of result that the CloudKit container event fetch request returns.

