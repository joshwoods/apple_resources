

- Core Data
- NSEntityDescription
-  insertNewObject(forEntityName:into:) 

Type Method

# insertNewObject(forEntityName:into:)

Creates, configures, and returns an instance of the class for the entity with a given name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func insertNewObject(
    forEntityName entityName: String,
    into context: NSManagedObjectContext
) -> NSManagedObject
```

## Parameters 

`entityName`  

The name of an entity.

`context`  

The managed object context to use.

## Return Value

A new, autoreleased, fully configured instance of the class for the entity named `entityName`. The instance has its entity description set and is inserted it into `context`.

## Discussion

This method makes it easy for you to create instances of a given entity without worrying about the details of managed object creation. The method is conceptually similar to the following code example.

```
NSManagedObjectModel *managedObjectModel =
        [[context persistentStoreCoordinator] managedObjectModel];
NSEntityDescription *entity =
        [[managedObjectModel entitiesByName] objectForKey:entityName];
NSManagedObject *newObject = [[NSManagedObject alloc]
            initWithEntity:entity insertIntoManagedObjectContext:context];
return newObject;
```

## See Also

### Related Documentation

init(entity: NSEntityDescription, insertInto: NSManagedObjectContext?)

Initializes a managed object from an entity description and inserts it into the specified managed object context.

