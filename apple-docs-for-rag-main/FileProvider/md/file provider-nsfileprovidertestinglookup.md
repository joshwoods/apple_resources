

- File Provider
-  NSFileProviderTestingLookup 

Protocol

# NSFileProviderTestingLookup

An operation that looks up an item.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
protocol NSFileProviderTestingLookup : NSFileProviderTestingOperation
```

## Topics

### Accessing the Operation’s Data

var itemIdentifier: NSFileProviderItemIdentifier

The unique identifier for the item.

**Required**

var side: NSFileProviderTestingOperationSide

The location where the lookup occurs.

**Required**

## Relationships

### Inherits From

- NSFileProviderTestingOperation
- NSObjectProtocol

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

protocol NSFileProviderTestingModification

An operation that syncs the modification of the source item to the target location.

protocol NSFileProviderTestingOperation

An operation that the system can schedule.

protocol NSFileProviderUserInteractionSuppressing

Support for suppressing user-interaction alerts.

enum NSFileProviderTestingOperationSide

The location where the operation takes place.

enum NSFileProviderTestingOperationType

The action that an operation performs.

com.apple.developer.fileprovider.testing-mode

A Boolean value that indicates whether you can place domains in testing mode.

