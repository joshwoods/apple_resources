

- Core Data
- NSEntityDescription
-  entity(forEntityName:in:) 

Type Method

# entity(forEntityName:in:)

Returns the entity with the specified name from the managed object model associated with the specified managed object context’s persistent store coordinator.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func entity(
    forEntityName entityName: String,
    in context: NSManagedObjectContext
) -> NSEntityDescription?
```

## Parameters 

`entityName`  

The name of an entity.

`context`  

The managed object context to use. Must not be `nil`.

## Return Value

The entity with the specified name from the managed object model associated with `context`’s persistent store coordinator.

## Discussion

Raises internalInconsistencyException if `context` is `nil`.

This method is functionally equivalent to the following code example.

```
NSManagedObjectModel *managedObjectModel = [[context persistentStoreCoordinator] managedObjectModel];
NSEntityDescription *entity = [[managedObjectModel entitiesByName] objectForKey:entityName];
return entity;
```

## See Also

### Related Documentation

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

