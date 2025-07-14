

- Core Data
- NSManagedObject
-  isDeleted 

Instance Property

# isDeleted

A Boolean value that indicates whether the managed object will be deleted during the next save.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isDeleted: Bool { get }
```

## Discussion

true if Core Data will ask the persistent store to delete the object during the next save operation, otherwise false. It may return false at other times, particularly after the object has been deleted. The immediacy with which it will stop returning true depends on where the object is in the process of being deleted.

If the receiver is a fault, accessing this property does not cause it to fire.

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

var isFault: Bool

A Boolean value that indicates whether the managed object is a fault.

var faultingState: Int

The faulting state of the managed object.

func hasFault(forRelationshipNamed: String) -> Bool

Returns a Boolean value that indicates whether the relationship for a given key is a fault.

var hasPersistentChangedValues: Bool

A Boolean value that indicates whether the managed object has persistent changes.

