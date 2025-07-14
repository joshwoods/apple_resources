

- Core Data
- NSManagedObject
-  hasFault(forRelationshipNamed:) 

Instance Method

# hasFault(forRelationshipNamed:)

Returns a Boolean value that indicates whether the relationship for a given key is a fault.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func hasFault(forRelationshipNamed key: String) -> Bool
```

## Parameters 

`key`  

The name of one of the receiver’s relationships.

## Return Value

true if the relationship for `key` is a fault; otherwise, false.

## Discussion

If the specified relationship is a fault, calling this method does not result in the fault firing.

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

var hasPersistentChangedValues: Bool

A Boolean value that indicates whether the managed object has persistent changes.

