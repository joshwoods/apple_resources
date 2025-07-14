

- Core Data
-  NSFetchedResultsChangeType 

Enumeration

# NSFetchedResultsChangeType

Constants that specify the possible types of changes that are reported.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum NSFetchedResultsChangeType
```

## Topics

### Constants

case insert

Specifies that an object was inserted.

case delete

Specifies that an object was deleted.

case move

Specifies that an object was moved.

case update

Specifies that an object was changed.

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

### Responding to Changes

protocol NSFetchedResultsControllerDelegate

A delegate protocol that describes the methods that the associated fetched results controller calls when the fetch results change.

protocol NSFetchedResultsSectionInfo

A protocol that defines the interface for section objects vended by a fetched results controller.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

