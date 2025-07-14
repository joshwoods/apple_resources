

- Core Data
-  NSBatchInsertRequestResultType 

Enumeration

# NSBatchInsertRequestResultType

Result types for a batch-insertion request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum NSBatchInsertRequestResultType
```

## Topics

### Request Types

case statusOnly

A value that indicates that the return type is a Boolean value representing whether the batch-insertion request succeeded.

case objectIDs

A value that indicates the return type is an array of object IDs that corresponds to the inserted rows.

case count

A value that indicates that the return type is the number of inserted rows.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Results

var result: Any?

The result of a batch-insertion request.

var resultType: NSBatchInsertRequestResultType

The type of result that Core Data returns from this request.

