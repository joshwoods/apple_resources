

- Core Data
- NSIncrementalStore
-  managedObjectContextDidRegisterObjects(with:) 

Instance Method

# managedObjectContextDidRegisterObjects(with:)

Indicates that objects identified by a given array of object IDs are in use in a managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func managedObjectContextDidRegisterObjects(with objectIDs: [NSManagedObjectID])
```

## Parameters 

`objectIDs`  

An array of object IDs.

## Discussion

This method and managedObjectContextDidUnregisterObjects(with:) allow managed object contexts to communicate interest in the row data of specific objects in a manner akin to reference counting. For more details, see managedObjectContextDidUnregisterObjects(with:).

## See Also

### Responding to Context Changes

func managedObjectContextDidUnregisterObjects(with: [NSManagedObjectID])

Indicates that objects identified by a given array of object IDs are no longer being used by a managed object context.

