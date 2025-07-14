

- Core Data
- NSManagedObject
-  hasChanges 

Instance Property

# hasChanges

A Boolean value that indicates whether the managed object has been inserted, has been deleted, or has unsaved changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var hasChanges: Bool { get }
```

## Discussion

true if the receiver has been inserted, has been deleted, or has unsaved changes, otherwise false. The result is the equivalent of OR-ing the values of isInserted, isDeleted, and isUpdated.

## See Also

### Getting State Information

var managedObjectContext: NSManagedObjectContext?

The managed object context with which the managed object is registered.

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

var hasPersistentChangedValues: Bool

A Boolean value that indicates whether the managed object has persistent changes.

