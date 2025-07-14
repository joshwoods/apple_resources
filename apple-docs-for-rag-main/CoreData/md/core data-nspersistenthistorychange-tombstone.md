

- Core Data
- NSPersistentHistoryChange
-  tombstone 

Instance Property

# tombstone

A dictionary of attributes marked for preservation after deletion, and their values when deleted.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var tombstone: [AnyHashable : Any]? { get }
```

## Mentioned in 

Consuming relevant store changes

## Discussion

This value is expected on changes of type NSPersistentHistoryChangeType.delete.

## See Also

### Inspecting Change Details

var changeID: Int64

The change’s numeric identifier.

var changeType: NSPersistentHistoryChangeType

The type of change to the managed object in the persistent store.

enum NSPersistentHistoryChangeType

The types of changes to managed objects reflected in persistent history.

var changedObjectID: NSManagedObjectID

The identifier of the managed object that changed. (swift) Declaration: @property(readonly, copy) NSManagedObjectID \*changedObjectID; (objc) Availability: iOS: 11.0 — iPadOS: 11.0 — Mac Catalyst: 13.1 — macOS: 10.13 — tvOS: 11.0 — visionOS: 1.0 — watchOS: 4.0 (objc,swift) }

var transaction: NSPersistentHistoryTransaction?

The persistent history transaction containing this change.

var updatedProperties: Set&lt;NSPropertyDescription>?

The set of properties that were updated on the managed object.

