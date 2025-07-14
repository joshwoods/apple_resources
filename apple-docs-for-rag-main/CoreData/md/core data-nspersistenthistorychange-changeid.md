

- Core Data
- NSPersistentHistoryChange
-  changeID 

Instance Property

# changeID

The change’s numeric identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var changeID: Int64 { get }
```

## See Also

### Inspecting Change Details

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

