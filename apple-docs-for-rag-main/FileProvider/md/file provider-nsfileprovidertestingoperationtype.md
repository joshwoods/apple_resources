

- File Provider
-  NSFileProviderTestingOperationType 

Enumeration

# NSFileProviderTestingOperationType

The action that an operation performs.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
enum NSFileProviderTestingOperationType
```

## Topics

### Types

case childrenEnumeration

Lists an item’s content.

case collisionResolution

Resolves a collision by renaming the new item.

case contentFetch

Fetches an item’s content.

case creation

Propagates the creation of a source item to the target location.

case deletion

Propagates the deletion of the source item from the target location.

case ingestion

Alerts the system to changes to either the local or remote storage.

case lookup

Looks up an item.

case modification

Propagates a change from the source item to the target location.

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

### Testing protocols

protocol NSFileProviderTestingChildrenEnumeration

An operation that lists a directory’s content.

protocol NSFileProviderTestingCollisionResolution

An operation that resolves a collision by renaming the new item.

protocol NSFileProviderTestingContentFetch

An operation that fetches an item’s content.

protocol NSFileProviderTestingCreation

An operation that syncs the creation of the source item to the target location.

protocol NSFileProviderTestingDeletion

An operation that syncs the deletion of the source item to the target location.

protocol NSFileProviderTestingIngestion

An operation that alerts the system to either local or remote storage changes.

protocol NSFileProviderTestingLookup

An operation that looks up an item.

protocol NSFileProviderTestingModification

An operation that syncs the modification of the source item to the target location.

protocol NSFileProviderTestingOperation

An operation that the system can schedule.

protocol NSFileProviderUserInteractionSuppressing

Support for suppressing user-interaction alerts.

enum NSFileProviderTestingOperationSide

The location where the operation takes place.

com.apple.developer.fileprovider.testing-mode

A Boolean value that indicates whether you can place domains in testing mode.

