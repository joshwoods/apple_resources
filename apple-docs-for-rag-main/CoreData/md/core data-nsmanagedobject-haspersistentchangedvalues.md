

- Core Data
- NSManagedObject
-  hasPersistentChangedValues 

Instance Property

# hasPersistentChangedValues

A Boolean value that indicates whether the managed object has persistent changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var hasPersistentChangedValues: Bool { get }
```

## See Also

### Getting State Information

var managedObjectContext: NSManagedObjectContext?

The managed object context with which the managed object is registered.

var hasChanges: Bool

A Boolean value that indicates whether the managed object has been inserted, has been deleted, or has unsaved changes.

var isInserted: Bool

A Boolean value that indicates whether the managed object has been inserted in a managed object context.

var isUpdated: Bool

A Boolean value that indicates whether the managed object has unsaved changes.

var isDeleted: Bool

A Boolean value that indicates whether the managed object will be deleted during the next save.

var isFault: Bool

A Boolean value that indicates whether the managed object is a fault.

var faultingState: Int

The faulting state of the managed object.

func hasFault(forRelationshipNamed: String) -> Bool

Returns a Boolean value that indicates whether the relationship for a given key is a fault.

