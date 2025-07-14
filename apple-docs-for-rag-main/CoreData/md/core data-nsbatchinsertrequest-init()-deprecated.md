

- Core Data
- NSBatchInsertRequest
-  init() Deprecated

Initializer

# init()

Creates a Core Data batch-insertion request.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.15–11.0DeprecatedtvOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–7.0Deprecated

``` source
convenience init()
```

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

init(entityName: String, objects: [[String : Any]])

Creates a batch-insertion request for a named managed entity, and provides an array of data dictionaries for insertion.

