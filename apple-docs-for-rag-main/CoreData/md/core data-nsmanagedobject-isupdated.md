

- Core Data
- NSManagedObject
-  isUpdated 

Instance Property

# isUpdated

A Boolean value that indicates whether the managed object has unsaved changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isUpdated: Bool { get }
```

## Discussion

true if the receiver has unsaved changes, otherwise false. The receiver has unsaved changes if it has been updated since its managed object context was last saved.

If the receiver is a fault, accessing this property does not cause it to fire.

## See Also

### Getting State Information

var managedObjectContext: NSManagedObjectContext?

The managed object context with which the managed object is registered.

var hasChanges: Bool

A Boolean value that indicates whether the managed object has been inserted, has been deleted, or has unsaved changes.

var isInserted: Bool

A Boolean value that indicates whether the managed object has been inserted in a managed object context.

var isDeleted: Bool

A Boolean value that indicates whether the managed object will be deleted during the next save.

var isFault: Bool

A Boolean value that indicates whether the managed object is a fault.

var faultingState: Int

The faulting state of the managed object.

func hasFault(forRelationshipNamed: String) -> Bool

Returns a Boolean value that indicates whether the relationship for a given key is a fault.

var hasPersistentChangedValues: Bool

A Boolean value that indicates whether the managed object has persistent changes.

