

- Core Data
-  NSBatchUpdateRequestResultType 

Enumeration

# NSBatchUpdateRequestResultType

Result types for a batch-update request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum NSBatchUpdateRequestResultType
```

## Topics

### Request Types

case statusOnlyResultType

A value that indicates the return type is a Boolean value representing whether the batch-update request succeeds.

case updatedObjectIDsResultType

A value that indicates the return type is an array of object IDs that corresponds to the updated rows.

case updatedObjectsCountResultType

A value that indicates the return type is the number of updated rows.

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

The result of a batch-update request, either the number of updated objects, the identifiers of the updated objects, or a status value.

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

