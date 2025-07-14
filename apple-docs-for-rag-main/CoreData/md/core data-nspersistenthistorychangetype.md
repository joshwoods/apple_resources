

- Core Data
-  NSPersistentHistoryChangeType 

Enumeration

# NSPersistentHistoryChangeType

The types of changes to managed objects reflected in persistent history.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum NSPersistentHistoryChangeType
```

## Topics

### Change Types

case delete

The deletion of a managed object from the persistent store.

case insert

The insertion of a managed object into the persistent store.

case update

An update to a managed object’s properties in the persistent store.

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

### Inspecting Change Details

var changeID: Int64

The change’s numeric identifier.

var changeType: NSPersistentHistoryChangeType

The type of change to the managed object in the persistent store.

var changedObjectID: NSManagedObjectID

The identifier of the managed object that changed. (swift) Declaration: @property(readonly, copy) NSManagedObjectID \*changedObjectID; (objc) Availability: iOS: 11.0 — iPadOS: 11.0 — Mac Catalyst: 13.1 — macOS: 10.13 — tvOS: 11.0 — visionOS: 1.0 — watchOS: 4.0 (objc,swift) }

var tombstone: [AnyHashable : Any]?

A dictionary of attributes marked for preservation after deletion, and their values when deleted.

var transaction: NSPersistentHistoryTransaction?

The persistent history transaction containing this change.

var updatedProperties: Set&lt;NSPropertyDescription>?

The set of properties that were updated on the managed object.

