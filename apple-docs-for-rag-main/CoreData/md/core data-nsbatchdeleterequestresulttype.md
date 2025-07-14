

- Core Data
-  NSBatchDeleteRequestResultType 

Enumeration

# NSBatchDeleteRequestResultType

The types of result a batch delete request can provide when it executes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NSBatchDeleteRequestResultType
```

## Topics

### Result Types

case resultTypeCount

Returns the number of managed objects the request deletes.

case resultTypeObjectIDs

Returns an array of the deleted managed objects’ identifiers.

case resultTypeStatusOnly

Returns a Boolean value that indicates if the request succeeds.

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

### Configuring the Result Type

var resultType: NSBatchDeleteRequestResultType

The type of result the request provides when it executes.

