

- Core Data
- NSIncrementalStore
-  managedObjectContextDidUnregisterObjects(with:) 

Instance Method

# managedObjectContextDidUnregisterObjects(with:)

Indicates that objects identified by a given array of object IDs are no longer being used by a managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func managedObjectContextDidUnregisterObjects(with objectIDs: [NSManagedObjectID])
```

## Parameters 

`objectIDs`  

An array of object IDs.

## Discussion

This method is the counterpart to managedObjectContextDidRegisterObjects(with:).

Passing an object ID in the object IDs array of managedObjectContextDidRegisterObjects(with:) is akin to incrementing the object ID’s reference count by 1; passing an object ID in the object IDs array of managedObjectContextDidUnregisterObjects(with:) is akin to decrementing the object ID’s reference count by 1. It is only when an object ID’s reference count is 0 that no contexts indicate that they are using the corresponding managed object. (Object IDs start with a reference count of 0.)

For example, if the register methods is invoked on two occasions when the object IDs array contains a given object ID, and the unregister method is invoked once when the object IDs array contains that object ID, then a context is still using the object with the given ID.

## See Also

### Responding to Context Changes

func managedObjectContextDidRegisterObjects(with: [NSManagedObjectID])

Indicates that objects identified by a given array of object IDs are in use in a managed object context.

