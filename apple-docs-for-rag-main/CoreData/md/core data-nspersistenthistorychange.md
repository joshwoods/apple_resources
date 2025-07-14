

- Core Data
-  NSPersistentHistoryChange 

Class

# NSPersistentHistoryChange

A change representing the insertion, update, or deletion of a managed object in the persistent store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSPersistentHistoryChange
```

## Mentioned in 

Consuming relevant store changes

## Topics

### Inspecting Change Metadata

class var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

A fetch request that has the persistent history change as the entity.

class var entityDescription: NSEntityDescription?

The entity description of the persistent history change entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description for the managed object type affected by the change using the provided context.

### Inspecting Change Details

var changeID: Int64

The change’s numeric identifier.

var changeType: NSPersistentHistoryChangeType

The type of change to the managed object in the persistent store.

enum NSPersistentHistoryChangeType

The types of changes to managed objects reflected in persistent history.

var changedObjectID: NSManagedObjectID

The identifier of the managed object that changed. (swift) Declaration: @property(readonly, copy) NSManagedObjectID \*changedObjectID; (objc) Availability: iOS: 11.0 — iPadOS: 11.0 — Mac Catalyst: 13.1 — macOS: 10.13 — tvOS: 11.0 — visionOS: 1.0 — watchOS: 4.0 (objc,swift) }

var tombstone: [AnyHashable : Any]?

A dictionary of attributes marked for preservation after deletion, and their values when deleted.

var transaction: NSPersistentHistoryTransaction?

The persistent history transaction containing this change.

var updatedProperties: Set&lt;NSPropertyDescription>?

The set of properties that were updated on the managed object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Reading History

class NSPersistentHistoryTransaction

A set of changes in the persistent history based on a context save or batch operation.

