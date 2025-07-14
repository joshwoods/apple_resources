

- Core Data
- NSBatchInsertRequest
-  init(entityName:objects:) 

Initializer

# init(entityName:objects:)

Creates a batch-insertion request for a named managed entity, and provides an array of data dictionaries for insertion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    entityName: String,
    objects dictionaries: [[String : Any]]
)
```

## Parameters 

`entityName`  

The name of the managed entity to insert data into.

`dictionaries`  

An array of dictionaries that represents objects to insert. Each dictionary contains an attribute name key and a value.

## Return Value

A batch-insertion request.

## See Also

### Creating a Request

convenience init(entity: NSEntityDescription, dictionaryHandler: (NSMutableDictionary) -> Bool)

Creates a batch-insertion request for a managed entity, and specifies a closure that provides data dictionaries for insertion.

convenience init(entity: NSEntityDescription, managedObjectHandler: (NSManagedObject) -> Bool)

Creates a batch-insertion request for a managed entity, and specifies a closure that inserts data into the entity.

convenience init(entityName: String, dictionaryHandler: (NSMutableDictionary) -> Bool)

Creates a batch-insertion request for a named managed entity, and specifies a closure that provides data dictionaries for insertion.

convenience init(entityName: String, managedObjectHandler: (NSManagedObject) -> Bool)

Creates a batch-insertion request for a named managed entity, and specifies a closure that inserts data into the entity.

init(entity: NSEntityDescription, objects: [[String : Any]])

Creates a batch-insertion request for a managed entity, and provides an array of data dictionaries for insertion.

convenience init()

Creates a Core Data batch-insertion request.

Deprecated

